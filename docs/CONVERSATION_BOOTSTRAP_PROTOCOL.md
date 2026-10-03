# Conversation Bootstrap Protocol

## Purpose

A consulting engagement should not require a handcrafted opening prompt every time a new ChatGPT conversation is started.

The portable process defines **how a conversation resolves its context**. The client control plane defines **the live context to resolve**.

## Operator experience

For a configured engagement, the user should be able to say:

> Check Tenshodo-Process and execute Engagement Step 2 for <client>.

Or:

> Check Tenshodo-Process and execute the current engagement step for <client>.

The short command is only a routing instruction. It is not the substantive work context.

## Repository roles

A client may have many repositories.

Only one should be the **engagement control plane** for a given engagement.

### Control-plane repository

Contains:

- `PROCESS_CONTEXT.json`;
- live client state;
- current executor / role conversation;
- authority and adoption metadata;
- current task and exact next action.

### Non-control client repository

May contain specialized project, application, code, data, or supporting work.

A non-control repo may include `PROCESS_POINTER.json`, which immediately identifies the client control-plane repository.

Use `templates/PROCESS_POINTER.json`.

## Portable layer — Tenshodo Process

The Process repository contains the engagement-step registry, bootstrap protocol, context/pointer templates, resolution rules, authority safeguards, and recovery behavior.

It contains no live confidential client state.

## Client layer — client control plane

Each configured client control-plane repository contains `PROCESS_CONTEXT.json`.

That packet identifies:

- process repository;
- client name and aliases;
- client control repository;
- live state file;
- current engagement step;
- current role conversation / executor;
- role START_HERE and charter;
- required read order;
- authority/adoption boundary;
- expected current task pointer;
- recovery rule.

The packet is pointer-oriented and must not duplicate live client state.

## Stable engagement-step IDs

- **ENG-01 — Establish engagement context**
- **ENG-02 — Resolve and launch the current work conversation**
- **ENG-03 — Execute bounded client work and checkpoint**
- **ENG-04 — Route decisions / adoption**
- **ENG-05 — Transfer or rotate stewardship**
- **ENG-06 — Close or transition the engagement**

Humans may say "Step 2"; the resolver maps ordinal 2 to `ENG-02`.

Do not renumber stable IDs after publication.

## Client-repository resolution algorithm

When the user names a client but not an exact control-plane repository:

1. Normalize the requested client name.
2. Inspect obvious matching repositories **only for small routing files first**:
   - `PROCESS_CONTEXT.json`;
   - `PROCESS_POINTER.json`.
3. If `PROCESS_CONTEXT.json` exists and its `client` or `client_aliases` matches, use that repository as the control plane.
4. If `PROCESS_POINTER.json` exists and its client matches, follow `client_control_repository` directly.
5. If the first obvious repo has neither routing file, search connected/installed repositories for `PROCESS_CONTEXT.json` whose `client` or `client_aliases` matches.
6. If exactly one matching control plane is found, use it.
7. If multiple matching control planes remain, ask only for the engagement/control repository needed to disambiguate.
8. Do **not** read large project plans or state files merely to discover where the control plane is if a routing file can answer the question.

This resolution order exists to minimize connector calls and startup latency.

## ENG-02 resolution algorithm

When asked to execute Step 2:

1. Read `engagement/STEP_REGISTRY.json` in Tenshodo Process.
2. Resolve Step 2 to `ENG-02`.
3. Resolve the client control-plane repository using the repository-resolution algorithm above.
4. Read that repository's `PROCESS_CONTEXT.json`.
5. Verify:
   - declared process repository is Tenshodo Process;
   - client name/alias matches;
   - current engagement step is compatible with ENG-02;
   - client state file exists;
   - current executor / role conversation is still active;
   - referenced START_HERE and charter exist.
6. Read the live client state file.
7. Reconcile the context packet against live state.
8. If live state differs, **live client state wins** and the discrepancy is checkpointed.
9. Read the role-specific START_HERE and charter.
10. Adopt the role-conversation identity named by live state.
11. Execute only work allowed by that role's execution class and authority boundary.
12. Continue into ENG-03 behavior: bounded work + durable checkpointing.

## Precedence

Highest to lowest:

1. live authoritative client systems for the information classes they own;
2. live client control-plane state and adopted decisions;
3. client `PROCESS_CONTEXT.json`;
4. non-control `PROCESS_POINTER.json`;
5. portable Process step definition;
6. human short launch phrase;
7. prior chat memory.

## Context-packet invariants

`PROCESS_CONTEXT.json` must be small, pointer-oriented, machine-readable, safe to read at startup, updated when routing changes, free of unnecessary confidential content, and consistent with live client state.

It must not become a second copy of client state.

## Pointer invariants

`PROCESS_POINTER.json` contains only enough information to redirect a conversation to the client control plane.

It should not include current task, people records, confidential business state, or detailed authority metadata.

## Recovery

If a context packet is missing or stale:

1. do not invent the role or task;
2. look for a repository pointer;
3. reconcile from the client zero-context handoff/state;
4. repair the context packet if authorized.

If a non-control repo is mistaken for the control plane:

1. check `PROCESS_POINTER.json`;
2. follow the pointer;
3. do not begin specialized-project work unless the resolved client state assigns it.

If no control plane can be identified after pointer/context discovery, ask only for the repository identifier needed to disambiguate.

## Definition of success

A user can open a fresh conversation, connect the relevant repositories, give a one-line step instruction, and the conversation can reconstruct the correct client control plane, role, mission, current task, required sources, authority boundaries, and checkpoint behavior without the user manually copying prior conversation context.

## Role-binding resolution

After resolving the client control plane and before substantive work, read `docs/ROLE_ROUTING_GUARD.md` and determine the conversation binding state.

- A fresh conversation is `unbound` and may adopt the live authorized executor role.
- A conversation already bound to the live executor is `bound_correct` and may continue within charter.
- A conversation bound to another role is `bound_wrong` and must not perform the live task or switch roles in the same chat.

When `bound_wrong`, provide the correct live role, current task, and exact handoff instruction. Shared facts may cross roles only through durable client state or another declared authoritative source.

After every substantive bounded batch, follow the Next-Step Contract in `docs/ROLE_ROUTING_GUARD.md` so the executing conversation itself tells the human operator whether to stay in the same chat, open a new chat, return to another role chat, provide a human decision, or stop because the engagement is complete.
