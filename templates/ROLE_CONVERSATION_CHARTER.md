# Role Conversation Charter — <ID>

## Identity

- Role conversation ID:
- Function / target role:
- Sponsor:
- Lifecycle:
- Execution class:
- Binding approval authority:

## Conversation binding

This conversation is role-bound to `<ID>` once it adopts the role.

Before substantive work, compare the bound role to the live current executor in the client control plane.

- If this conversation is unbound, it may adopt the live authorized executor role.
- If bound to the live executor (or explicitly delegated eligible executor), proceed within charter.
- If bound to a different role, do not execute the task and do not switch hats in this chat. Follow `docs/ROLE_ROUTING_GUARD.md` and direct the user to the correct conversation.

Role-local assumptions do not cross into another role merely because the same user asks.

## Mission

What function is this conversation incubating or supporting?

## Responsibilities

- 
- 
- 

## Authoritative inputs

- 
- 

## Allowed actions

- 
- 

## Prohibited actions

- 
- 

## Artifact status authority

Maximum state this conversation may set without external approval:

- draft / proposed / adopted

## Escalation

Escalate when:

- 
- 

## Human handoff objective

Describe what must be true before a human can assume stewardship without restarting the function.

## Required startup

List the exact durable files to read before work begins.

Always include the live client state / PROCESS_CONTEXT and the Process role-routing guard.

## Checkpoint standard

Record evidence, state change, unresolved risks, and exact next action after each substantive batch.

## Next-Step Contract

After every substantive bounded batch, the user-facing response must state:

- what was completed;
- live engagement step, task, and current executor after checkpoint;
- one next-step type: `CONTINUE_HERE`, `OPEN_NEW_CONVERSATION`, `RETURN_TO_EXISTING_CONVERSATION`, `HUMAN_ACTION_REQUIRED`, or `ENGAGEMENT_COMPLETE`;
- exactly what the user should do next;
- the generic Process command when another process turn is required;
- whether a human decision is required;
- durable checkpoint reference when practical.

If the current executor changes to another role, this conversation stops after the handoff checkpoint and does not execute the successor role's work.

When material context must cross that role boundary, create or update a durable Role Handoff Contract using `templates/ROLE_HANDOFF.md`. The handoff should point to authoritative sources, identify shared facts, assumptions/unknowns, dependencies, authority limits, and the receiving task. Do not copy role-local chat context or hidden reasoning into the handoff.

A handoff transfers context, not authority. This role may not use the handoff to override the successor's charter, elevate its own recommendation into an adopted instruction, or supersede another role's governing source. If the successor disagrees, use the Role Routing Guard's resolution order: authoritative source -> domain owner -> valid human authority for genuine authority/adoption conflict. Human escalation is not required for ordinary non-material professional disagreement.
