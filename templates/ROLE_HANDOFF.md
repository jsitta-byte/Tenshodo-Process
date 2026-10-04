# Role Handoff Contract

Use this template when material work crosses from one governed role conversation to another and the receiving role needs shared operational context beyond a simple task pointer.

The handoff is not a transcript. It is a compact durable contract that states what the receiving role is allowed to inherit, where the authority for each fact lives, what remains unresolved, and what must happen next.

## Metadata

- Handoff ID:
- Client / engagement:
- Workstream:
- From role conversation:
- To role conversation:
- Trigger:
- Next-Step Contract type:
- Source checkpoint / commit:
- Handoff state: draft / proposed / acknowledged / superseded

## Completed scope

What did the sending role complete before handoff?

- Task / batch:
- Artifacts created or changed:
- Validation completed:
- Artifact states:

## Durable sources the receiving role should read

For each source, record the pointer and why it matters.

| Source | Authority / purpose | Version / checkpoint | Artifact state |
| --- | --- | --- | --- |
|  |  |  |  |

Do not restate an underlying fact as if the handoff itself were its authority. Point to the durable source that owns the fact.

## Shared facts crossing the role boundary

Record only facts that are already durable in an authoritative or declared shared source.

- 
- 

## Open assumptions, unknowns, and disputes

State what is not established.

- 
- 

## Context that must NOT cross implicitly

List role-local hypotheses, heuristics, preferences, or unfinished reasoning that the receiving role must not inherit as fact.

- 
- 

## Dependencies and escalations

| Dependency | Owner / role | Blocking class | Required resolution |
| --- | --- | --- | --- |
|  |  | hard / soft / consultation / adoption |  |

## Authority and adoption boundaries

- Current execution class:
- Maximum artifact state:
- Adoption authority:
- Prohibited commitments / decisions:
- Specialist review triggers:

## Receiving-role task

- Target task:
- Current batch:
- Exact objective:
- Definition of done:
- Exact next action:
- Operator command, if needed:

## Receipt / acknowledgement

The receiving role should verify live durable state before execution.

- Receiving role confirmed:
- Live state matched handoff: yes / no
- Reconciliation needed:
- Receipt checkpoint:

## Rules

1. A role handoff does not replace the live client control plane.
2. Live durable state and declared authoritative systems override the handoff if they differ.
3. Do not copy chat transcripts, hidden reasoning, or role-local assumptions into the handoff.
4. Cross-role facts must already exist in durable shared state or another declared authoritative source.
5. The handoff may summarize and route facts; it does not become a new authority for them.
6. Use a handoff when material context, dependencies, authority boundaries, or source pointers must cross roles. Do not create one for trivial same-role continuation.
7. Conversation routing and context transfer are separate concerns: the Next-Step Contract identifies where execution goes; this artifact defines what durable context may cross with it.
