# Role Handoff Contract

Use this template when material work crosses from one governed role conversation to another and the receiving role needs shared operational context beyond a simple task pointer.

The handoff is not a transcript, memory export, or command channel between roles. It is a compact durable contract that states what the receiving role is allowed to inherit, where the authority for each fact lives, what remains unresolved, and what must happen next.

**A handoff transfers context, not authority.**

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

## Context classification

Classify material context before it crosses the role boundary.

| Item | Class | Authoritative source / owner | Recipient treatment |
| --- | --- | --- | --- |
|  | authoritative fact / adopted decision / recommendation-hypothesis / dependency-request / unknown-disputed |  | follow source / may challenge / route / escalate |

Use these classes:

- **Authoritative fact** — already established by a declared authoritative source. The receiving role follows the source, not the sender's wording.
- **Adopted decision / sponsor direction** — validly adopted or sponsor-authorized direction recorded through the client's authority model. It governs only within its stated scope and remains subject to later valid supersession.
- **Recommendation / hypothesis** — sending-role judgment, preference, working theory, or proposed interpretation. It is non-binding. The receiving role may disagree, replace it within its own domain, or route it back for discussion.
- **Dependency / request** — work the sending role needs from another domain. It does not create authority over that domain.
- **Unknown / disputed** — not established. The receiving role must not treat it as fact.

A role title does not change these classes. Labels such as **Chief**, **Executive**, **Stakeholder**, **Lead**, or similar do not create cross-role override authority unless a separate durable authority record explicitly grants it.

## Shared facts crossing the role boundary

Record only facts that are already durable in an authoritative or declared shared source.

- 
- 

## Open assumptions, unknowns, and disputes

State what is not established.

- 
- 

## Context that must NOT cross implicitly

List role-local hypotheses, heuristics, preferences, unfinished reasoning, or non-durable instructions that the receiving role must not inherit as fact or command.

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
- Cross-role override authority, if any: none unless explicitly sourced below
- Explicit authority source, if applicable:

## Disagreement / conflict resolution

A receiving role may disagree with transferred context. Resolve disagreements in this order:

1. **Source-resolvable** — if authoritative durable sources answer the question, follow the declared source hierarchy, record the discrepancy when material, and continue.
2. **Domain-owned** — if the issue belongs to another role's governed domain and is not settled by an authoritative source, route the issue to that domain owner. The receiving role may propose a change but must not silently rewrite or supersede the other role's governing source.
3. **Authority / adoption conflict** — if authoritative sources conflict, authority is ambiguous, the requested change crosses decision rights, or resolution would create/supersede a consequential adopted decision, stop that consequential action and escalate to the valid human adoption authority, sponsor, or steward defined by the client authority model.
4. **Non-material professional disagreement** — record or resolve within the receiving role's own charter when no cross-domain authority or adoption decision is implicated. Human escalation is not required merely because roles disagree.

A human steward is not automatically the final authority. Escalate to the **valid human authority for the decision class**. The steward may coordinate that escalation when its charter permits.

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
- Context classification reviewed: yes / no
- Authority conflict found: yes / no
- Reconciliation / escalation needed:
- Receipt checkpoint:

## Rules

1. A role handoff does not replace the live client control plane.
2. Live durable state and declared authoritative systems override the handoff if they differ.
3. Do not copy chat transcripts, hidden reasoning, or role-local assumptions into the handoff.
4. Cross-role facts must already exist in durable shared state or another declared authoritative source.
5. The handoff may summarize and route facts; it does not become a new authority for them.
6. A sending role cannot use a handoff to expand its authority, narrow the receiving role's charter, or convert its recommendation into an adopted instruction.
7. A receiving role must not modify or supersede another role's governing source merely to resolve a handoff conflict unless its charter and a valid authority record explicitly permit that action.
8. Valid human direction may govern or supersede role context only within the human's declared authority and must be recorded durably when consequential.
9. Use a handoff when material context, dependencies, authority boundaries, or source pointers must cross roles. Do not create one for trivial same-role continuation.
10. Conversation routing and context transfer are separate concerns: the Next-Step Contract identifies where execution goes; this artifact defines what durable context may cross with it.
