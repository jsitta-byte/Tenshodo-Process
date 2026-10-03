# Method Principles

## 1. Conversation is not the system of record

Meetings, chats, LLM sessions, and agent runs execute work.

Durable state must live elsewhere.

## 2. Zero-context resumption is a design requirement

A qualified newcomer should be able to resume important work without asking the previous operator to reconstruct history.

The durable state should identify:

- current task;
- authority;
- dependencies;
- completed checkpoints;
- evidence;
- exact next action.

## 3. Separate working plane from durable control plane

Collaborative documents and active operational work may live in SharePoint, Google Workspace, CRM, finance systems, or other tools.

The durable control plane records the state and relationships needed to govern and resume that work.

Do not force every artifact into Git merely to make Git central.

## 4. One declared authority per information class

Parallel editable truths create reconciliation debt.

Each information class should have one declared authoritative source at a time, plus explicit replicas, exports, or transition rules where needed.

## 5. Revalidate live sources before crediting prior work

A checkpoint is evidence of what was true at checkpoint time.

If external source state can change, revalidate it before treating earlier classifications as current.

## 6. Bounded work is safer work

Long tasks should have deterministic batches and checkpoint boundaries.

A partial attempt is not completion.

## 7. Evidence beats conversational claims

Completion must be supported by durable artifacts or source evidence.

"Someone said it was done" is not a control.

## 8. Preserve distinct truth dimensions

Do not collapse dimensions merely because one data point is convenient.

A portable example:

- current system behavior;
- historical validity;
- current economic or operational conditions

may all be different truths requiring different evidence.

## 9. Target accountability is not current authority

A future org chart cannot authorize today's work.

Model:

- where responsibility should ultimately live;
- who is actually allowed to act now.

## 10. Bootstrap before the target organization exists

Transformation must remain executable when the roles the future model calls for do not yet exist.

Use narrow, temporary, reviewable transition mechanisms.

## 11. AI can incubate a function without becoming the executive

A role-based AI conversation may research, build, draft, map, test, and propose within an explicit charter.

It does not acquire human legal or organizational authority from the prompt.

## 12. Proposal and adoption are different states

Useful states include:

- draft;
- proposed;
- adopted;
- superseded.

An AI or consultant should not quietly convert its own proposal into binding policy unless current authority explicitly permits it.

## 13. Local improvement should create global awareness

An employee should be able to propose a local improvement.

The system should identify likely downstream impacts across processes, systems, controls, products, training, documents, and roles.

Impact discovery is not automatic approval.

## 14. Human takeover is a handoff, not a restart

If consultants or AI build a function, the future human steward inherits:

- durable state;
- source rules;
- open tasks;
- decisions;
- risks;
- exact next action.

## 15. Portability is earned

A pattern is not portable because it is elegant.

It becomes portable when evidence shows it survives differences in organization, tools, culture, authority, and domain.

## 16. Escalate uncertainty, not meetings

> **Do not interview people for facts the organization can already prove. Do not infer facts the organization can cheaply confirm. Do not redesign the organization until you understand enough of the work and authority that actually exist.**

Discovery should use the least expensive reliable evidence source first:

authoritative system → controlled record → observed operational evidence → provisional inference → asynchronous confirmation → manager/owner confirmation → consultant interview/workshop.

Inference is a fallback and accelerator, not a substitute for evidence.

Human consulting time should concentrate on high-consequence ambiguity, disagreement, undocumented authority, hidden process behavior, and transformation-critical unknowns.

## 17. Model working-plane topology, not a provider assumption

An organization may have one working environment or many.

Model the actual topology as distinct provider, tenant/account, environment, service, and location identities. Do not treat a provider name such as SharePoint, Google Drive, or GitHub as sufficient environment identity.

Authority is assigned separately by information class.

A matching artifact found in the wrong tenant, environment, or location is not valid evidence merely because its name or contents look relevant.

## 18. Discovery depth should match organizational maturity

Do not force every organization through the same discovery burden.

Prefer the least intrusive evidence path that can establish a trustworthy baseline:

- mature process corpus / authoritative structured records;
- corpus plus targeted connected validation;
- broader authorized connected discovery when documentation is weak;
- targeted human validation for consequential remaining uncertainty.

Connected discovery is optional, scoped, and normally read-only.

## 19. Connected discovery accelerates evidence collection; it does not create authority

Authorized AI access may reconstruct candidate processes, systems, handoffs, artifacts, Benchmarks, controls, and SOPs from operating evidence.

Observed behavior and AI inference remain evidence states, not adopted organizational truth.

Generated SOPs, process descriptions, authority maps, and Benchmarks remain draft or proposed until the appropriate validation and adoption occur.

## 20. Capture method learning before memory becomes the dependency

A reusable lesson discovered during client execution must not depend on the participants remembering to reconstruct it later.

Capture the observation durably first.

Triage, abstraction, evidence calibration, and method adoption may occur later.

The active methodology cursor should continue independently from the observation queue.
