# Engagement Conversation Quick Start

## Normal operator command

Once a client is configured, starting the next governed conversation should require only a short instruction.

Preferred form:

> **Check Tenshodo-Process and execute Engagement Step 2 for <client>.**

Equivalent stable-ID form:

> **Check Tenshodo-Process and execute ENG-02 for <client>.**

If the connected workspace already makes the client unambiguous:

> **Check the process and execute Step 2.**

## Even shorter continuation form

After an engagement is fully configured, operators may say:

> **Check Tenshodo-Process and execute the current engagement step for <client>.**

The resolver should inspect the client's routing files and live state rather than asking the user to remember the current step number.

## What happens automatically

For Step 2, the conversation:

1. reads `engagement/STEP_REGISTRY.json`;
2. resolves Step 2 → `ENG-02`;
3. reads `docs/CONVERSATION_BOOTSTRAP_PROTOCOL.md`;
4. resolves the correct client control-plane repository;
5. checks small routing files first:
   - `PROCESS_CONTEXT.json`;
   - `PROCESS_POINTER.json`;
6. follows a pointer immediately if the named repository is a specialized/non-control repo;
7. reads the control plane's `PROCESS_CONTEXT.json`;
8. validates it against live client state;
9. reads the current role START_HERE and charter;
10. adopts the live authorized role-conversation identity;
11. resumes the live eligible task;
12. checkpoints according to the client runbook.

## Multi-repository clients

A client may have many repositories.

The repo whose name most closely resembles the client name is **not necessarily** the engagement control plane.

Non-control repositories should include `PROCESS_POINTER.json` generated from `templates/PROCESS_POINTER.json`.

That pointer exists specifically to avoid exploratory reads of large project files during startup.

## Human input should be minimal

If the client cannot be inferred after context/pointer discovery, ask only for the client/control-repository identifier.

Do not ask the user to paste:

- the prior launch prompt;
- previous conversation history;
- the current role;
- the current task;
- authority rules;
- the role charter.

Those belong in durable state.

## Setup requirement

Each client control plane must include a valid `PROCESS_CONTEXT.json` generated from `templates/PROCESS_CONTEXT.json`.

Each related non-control repository should include a `PROCESS_POINTER.json` when its name could plausibly be mistaken for the engagement control plane.

The context packet is a pointer layer only. Live client state wins if the packet is stale.
