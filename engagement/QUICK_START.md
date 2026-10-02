# Engagement Conversation Quick Start

## Normal operator command

Once a client has a valid `PROCESS_CONTEXT.json`, starting the next governed conversation should require only a short instruction.

Preferred form:

> **Check Tenshodo-Process and execute Engagement Step 2 for <client>.**

Equivalent stable-ID form:

> **Check Tenshodo-Process and execute ENG-02 for <client>.**

If the connected workspace already makes the client unambiguous:

> **Check the process and execute Step 2.**

## Even shorter continuation form

After an engagement is fully configured, operators may say:

> **Check Tenshodo-Process and execute the current engagement step for <client>.**

The resolver should inspect the client's `PROCESS_CONTEXT.json` rather than asking the user to remember the current step number.

## What happens automatically

For Step 2, the conversation:

1. reads `engagement/STEP_REGISTRY.json`;
2. resolves Step 2 → `ENG-02`;
3. reads `docs/CONVERSATION_BOOTSTRAP_PROTOCOL.md`;
4. locates the client's control-plane repository;
5. reads client `PROCESS_CONTEXT.json`;
6. validates it against live client state;
7. reads the current role START_HERE and charter;
8. adopts the live authorized role-conversation identity;
9. resumes the live eligible task;
10. checkpoints according to the client runbook.

## Human input should be minimal

If the client cannot be inferred, ask only for the client/repository identifier.

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

The context packet is a pointer layer only. Live client state wins if the packet is stale.
