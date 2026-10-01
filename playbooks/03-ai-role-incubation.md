# Playbook 03 — AI Role Incubation

## Use when

A client needs a function before it has a clear human owner, mature job description, sufficient internal understanding, or staffing capacity.

## Concept

Create a chartered role conversation.

The conversation adopts the function's mission, perspective, source rules, work queue, output contract, checkpoint discipline, and escalation rules.

It does not become the executive.

## Required durable artifacts

Before launching a role conversation, establish:

- stable role-conversation ID;
- role charter;
- START_HERE or equivalent handoff;
- current state file;
- work plan;
- operating runbook;
- authority/adoption boundary;
- role-conversation registry entry;
- relevant decisions and worklog paths.

Use `templates/ROLE_CONVERSATION_CHARTER.md` for the charter.

Use `templates/ROLE_CONVERSATION_LAUNCH_PROMPT.md` to generate the opening ChatGPT command.

## Launch protocol

The opening prompt is an **ignition key**, not the operating record.

A valid launch prompt should:

1. identify the stable role-conversation ID;
2. point to the live client control repository;
3. require the conversation to read its handoff, charter, state, plan, runbook, authority model, decisions, and worklog;
4. require live-state verification before substantive work;
5. state that the repository and declared authoritative systems override the launch prompt;
6. verify the role has not been retired, superseded, or reassigned;
7. declare execution class, allowed actions, prohibited actions, maximum artifact state, and adoption authority;
8. require bounded checkpointing and zero-context handoff.

Do not paste extensive client history into the launch prompt merely to make the conversation feel informed.

Durable client context belongs in the client control plane and authoritative client systems.

## Stale-prompt safeguard

The conversation must verify role status, charter currentness, task assignment, execution class, adoption authority, and required live systems.

If the launch prompt conflicts with live durable state, live durable state wins and the discrepancy should be recorded.

## Allowed work

Typical build/propose work includes research, analysis, inventory, process architecture, documentation, dependency mapping, draft controls, recommendations, work planning, testing, evaluation, and durable checkpointing.

## Binding authority

Keep human or otherwise explicitly delegated.

A role conversation does not automatically hire/fire, set pay, spend, sign contracts, grant access, accept material risk, or adopt its own policy.

## Artifact-state boundary

Where consequential work requires state, prefer:

- draft;
- proposed;
- adopted;
- superseded.

A role conversation's maximum state without separate approval should be declared in its charter and launch prompt.

## Lifecycle

1. AI-incubated
2. human-supervised
3. human-led with AI copilot
4. formally staffed/delegated
5. retained as support or retired

## Handoff objective

The future human should inherit a working function, not a blank page.

## Definition of success

A zero-context ChatGPT conversation can be launched from the standard prompt, discover the authoritative current task and authority boundary, perform bounded work, checkpoint it durably, and be replaced without material knowledge loss.
