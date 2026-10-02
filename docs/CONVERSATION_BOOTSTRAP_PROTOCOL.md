# Conversation Bootstrap Protocol

## Purpose

A consulting engagement should not require a handcrafted opening prompt every time a new ChatGPT conversation is started.

The portable process defines **how a conversation resolves its context**.

The client control plane defines **the live context to resolve**.

This keeps the launch instruction small while preserving client confidentiality, live-state precedence, and zero-context resumability.

## The operator experience

For a configured engagement, the human should be able to start a new conversation with a short instruction such as:

> Check Tenshodo-Process and execute Engagement Step 2 for <client>.

Or, when the client repository is already obvious from workspace context:

> Check the process and execute Engagement Step 2.

The new conversation must not depend on the wording of that short command for substantive context.

It uses the command only to locate the durable process and client context packet.

## Two-layer design

### Portable layer — Tenshodo Process

The process repository contains:

- the engagement-step registry;
- the conversation-bootstrap protocol;
- context-packet schema/template;
- resolution rules;
- authority safeguards;
- recovery behavior.

It contains no live confidential client state.

### Client layer — client control plane

Each configured client repository contains a small durable file, normally:

`PROCESS_CONTEXT.json`

That file identifies:

- process method and version/ref;
- current engagement step;
- client repository;
- client state file;
- current role conversation / executor;
- role START_HERE and charter;
- required read order;
- authority/adoption boundary;
- exact current task pointer;
- recovery rule.

The context packet should point to live client artifacts rather than duplicate their contents.

## Stable engagement-step IDs

Use stable IDs rather than relying only on prose or a mutable ordinal.

The initial standard is:

- **ENG-01 — Establish engagement context**
- **ENG-02 — Resolve and launch the current work conversation**
- **ENG-03 — Execute bounded client work and checkpoint**
- **ENG-04 — Route decisions / adoption**
- **ENG-05 — Transfer or rotate stewardship**
- **ENG-06 — Close or transition the engagement**

Humans may say "Step 2"; the resolver maps ordinal 2 to `ENG-02`.

Do not renumber existing stable IDs after publication.

## ENG-02 resolution algorithm

When asked to execute Step 2:

1. Read `engagement/STEP_REGISTRY.json` in Tenshodo Process.
2. Resolve Step 2 to `ENG-02`.
3. Identify the client control-plane repository from:
   - an explicit repository/client in the user's command; or
   - the already connected/current engagement context.
4. Read the client repository's `PROCESS_CONTEXT.json`.
5. Verify:
   - its declared process repository is Tenshodo Process;
   - its current_engagement_step is compatible with ENG-02;
   - its client state file exists;
   - its current executor / role conversation is still active;
   - referenced START_HERE and charter exist.
6. Read the client live state file.
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
3. client PROCESS_CONTEXT.json;
4. portable Process step definition;
5. the human's short launch phrase;
6. prior chat memory.

The short launch phrase never overrides durable authority.

## Client context packet invariants

`PROCESS_CONTEXT.json` must be:

- small;
- pointer-oriented;
- machine-readable;
- safe to read at startup;
- updated whenever the current executor or process step changes;
- free of unnecessary confidential content;
- consistent with the client state file.

It must not become a second copy of client state.

## Recovery

If the context packet is missing or stale:

1. do not invent the role or task;
2. read the client zero-context handoff/state directly;
3. reconcile the correct executor and task;
4. repair PROCESS_CONTEXT.json as part of the checkpoint if authorized.

If no client repository can be identified, ask only for the client/repository identifier needed to resolve the context.

## Definition of success

A user can open a fresh conversation, connect the relevant repositories, give a one-line step instruction, and the conversation can reconstruct:

- its role;
- its mission;
- the current task;
- required sources;
- authority boundaries;
- checkpoint behavior;

without the user manually copying the prior conversation prompt.
