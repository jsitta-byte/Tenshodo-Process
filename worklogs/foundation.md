# Methodology Foundation Worklog

## 2026-10-01 — Consultancy methodology initialized

### Objective

Create a portable playbook so the Tenshodo management team can perform operating-system transformation across multiple organizations without carrying client-specific state between engagements.

### Established

- Public methodology repository boundary.
- Consultancy delivery model.
- Portable method principles.
- Engagement lifecycle.
- Client repository architecture.
- Confidentiality / clean-room rule.
- Evidence-based pattern maturity model.
- Machine-readable pattern registry.
- Human-readable evidence matrix.
- Initial reusable playbooks.
- Client starter templates.
- Sanitized field notes from Tenshodo Exchange.
- Machine-readable methodology state and roadmap.
- Methodology runbook so the process repository follows its own durability rules.
- DEC-0001 establishing the portable-method/client-state boundary.

## 2026-10-01 — Role-conversation launch standard captured

Captured a reusable launch prompt and established that live durable state overrides launch-prompt text.

## 2026-10-01 — M02 evidence calibration completed

Calibrated every active pattern with operating conditions, failure modes, limits, falsifiers, evidence locators, and portability gaps.

No pattern was promoted to Portable.

## 2026-10-02 — Process-driven conversation bootstrap established

Moved substantive launch context out of the human prompt and into a portable ENG-step resolver plus client `PROCESS_CONTEXT.json`.

## 2026-10-02 — Live Step-2 launch exposed repository ambiguity

A live launch test showed that a multi-repository client needs deterministic routing before substantive repository reads.

Added the `PROCESS_POINTER.json` pattern and hardened ENG-02 repository resolution.

## 2026-10-03 — Current-State Discovery SOP established; M03 completed

### Trigger

The live Tenshodo organizational-bootstrap work surfaced a recurring consulting question:

Should consultants infer people/process profiles first, design processes first, or interview everyone?

The emerging answer needed to become portable method before the next ten client engagements.

### Governing principle

> Do not interview people for facts the organization can already prove. Do not infer facts the organization can cheaply confirm. Do not redesign the organization until you understand enough of the work and authority that actually exist.

### Standard sequence

Evidence intake → current-process discovery → provisional inference → targeted validation → current-state baseline → transformation.

### Discovery modes

- document-led;
- hybrid;
- interview-led.

The mode changes the cost mix, not the underlying evidence/authority discipline.

### Evidence escalation ladder

1. authoritative business system;
2. controlled/documented record;
3. observed operational evidence;
4. AI/consultant inference;
5. asynchronous employee confirmation;
6. manager/accountable-owner confirmation;
7. consultant interview/workshop.

Consequential decision authority is excluded from inference-by-title/activity and remains documented, attested, unknown, or disputed.

### Discovery control artifacts created

- `playbooks/05-current-state-discovery.md`
- `templates/DISCOVERY_INTAKE_CHECKLIST.md`
- `templates/EXECUTIVE_SPONSOR_INTERVIEW.md`
- `templates/CURRENT_STATE_CONFIDENCE_MAP.json`
- `templates/CURRENT_STATE_DISCOVERY_ASSESSMENT.md`
- `templates/DISCOVERY_OUTPUT_CONTRACT.md`

### Completion

M03 definition of done is satisfied.

The discovery system now supports:

- clients that can drop off authoritative data immediately;
- clients that need a hybrid of evidence and validation;
- clients that require interview-led discovery;
- field-level inference with provenance/confidence;
- targeted use of consultants for high-consequence uncertainty.

### Exact next action

Execute M04: package the accepted discovery outputs into a reusable client control-plane bootstrap kit, including generic plan/runbook/worklog/authority artifacts and an assembly checklist.

## 2026-10-03 — Role-bound conversation routing established

### Problem

The one-line Process command made conversation startup easy, but a new risk remained: a user could send the same command to a chat already operating another governed role. Without a hard guard, an HR-oriented conversation might silently switch to technology work or carry role-local assumptions into another domain.

A second operator problem also remained: after each batch, the user still sometimes needed a separate supervisory conversation to determine whether to stay in the same chat or open a new role conversation.

### Established

- A governed chat is `unbound` until it adopts a role.
- Once adopted, the chat is role-bound for its lifetime.
- `bound_correct` conversations may proceed within charter.
- `bound_wrong` conversations must stop without performing the other role's work.
- Cross-role context must come through durable client state or another authoritative source.
- A role may create/charter its successor when assigned to do so, but must stop after durable state changes the executor.
- Every bounded batch must emit a Next-Step Contract with one of:
  - CONTINUE_HERE;
  - OPEN_NEW_CONVERSATION;
  - RETURN_TO_EXISTING_CONVERSATION;
  - HUMAN_ACTION_REQUIRED;
  - ENGAGEMENT_COMPLETE.

### Intended operator experience

The user should be able to rely on the executing conversation itself to say where to go next. If the user sends a prompt to the wrong role chat, that chat should protect the role/domain boundary and redirect the user rather than changing identities.


## 2026-10-03 — Parallel workstreams and commercialization architecture established

### Trigger

A live field-laboratory need exposed two methodology gaps:

1. the client operating system was approaching the point where COO, marketing, revenue, technology, and other functions could have real work at the same time;
2. commercialization work needed a reusable method rather than ad hoc creation of decks and brand assets.

### Parallel-workstream decision

Retain the simple single-cursor model for early engagements.

Add a workstream registry only when at least two durable bodies of work can proceed with distinct executors or independently useful checkpoints.

A workstream is a durable lane of work, not a role and not a second client control plane.

Role binding resolves before workstream routing.

### Commercialization decision

Commercialization is an optional module, not a mandatory stage for every transformation.

Activation is evidence-driven: real market-facing work must exist.

The module begins from durable source artifacts rather than collateral:

- Brand & Market Foundation;
- Offer Architecture;
- Claims / Proof Register;
- Sales Enablement Handoff.

Sales decks, marketing decks, one-pagers, websites, and campaigns are downstream assets generated from these sources.

### Functional separation

The portable module preserves distinctions among:

- product/service — what is being sold;
- marketing — for whom, why it matters, and how it is explained;
- revenue — how it is sold;
- finance — whether commercial economics are sound.

These target-accountability distinctions do not automatically activate executive role conversations.

### Exact next Process action

Continue M04 by completing the remaining generic client bootstrap artifacts and assembly checklist. Parallel-workstream and commercialization support are now available as reusable prework.

## 2026-10-03 — Multi-environment discovery architecture and method-learning loop captured

### Trigger

A live management-governance correction exposed two distinct method gaps:

1. provider-level or singular-working-plane language is insufficient when organizations can operate across multiple clouds, tenants, environments, services, and locations;
2. major 10XP improvements can emerge during client work while the methodology-development cursor is busy elsewhere.

A parallel integration discussion also exposed terminology drift between teams and the need to compare semantics before renaming durable concepts.

### Established

- Working-Plane Topology with provider → tenant/account → environment → service → location identity;
- separate Information Authority and Information Flow registries;
- optional, scope-controlled Connected Discovery with read-only default;
- mature-process-corpus shortcut before broad connector access;
- Process Evidence Graph for candidate process reconstruction;
- AI-drafted SOP and Benchmark candidates remain draft/proposed pending validation/adoption;
- wrong-environment search results are not evidence merely because they match;
- terminology crosswalk before source-system renaming;
- Method Observation queue so reusable lessons are captured immediately without changing the active methodology cursor.

### Pattern registration

Registered PAT-012 through PAT-015 as Candidate Patterns.

No portability promotion occurred.

### Cursor

M04 remains active. The new capabilities are additive prework and runtime support; they do not restart M03 or M04.

### Exact next Process action

Complete the remaining M04 generic client plan, runbook, worklog, authority/source model, adoption-status controls, and bootstrap assembly checklist.

## 2026-10-04 — Durable cross-role handoff contract

### Trigger

A client role transition was routed to the correct successor function in durable state, but the operator path deviated from the named existing conversation. Client reconciliation confirmed that the routing rule itself already existed and the successor activation remained substantively valid.

The broader method lesson was different: routing correctness does not by itself define what context should cross from one governed role to another.

### Method distinction

Two controls are now explicit:

1. **Next-Step Contract** — identifies where execution goes next.
2. **Role Handoff Contract** — identifies what durable context may cross with the transition.

The Role Handoff Contract is intentionally compact and source-oriented. It records:

- source/receiving roles and checkpoint;
- authoritative source pointers;
- durable shared facts;
- assumptions, unknowns, and disputes;
- context that must not cross implicitly;
- dependencies/escalations;
- authority/adoption boundaries;
- receiving task, exact next action, and completion condition.

It does not copy transcripts, hidden reasoning, or role-local working context.

### Artifacts

Added:
- `templates/ROLE_HANDOFF.md`;
- MOBS-005 in the Method Observation Register;
- PAT-016 Durable cross-role handoff contract as Candidate Pattern.

Updated:
- Role Routing Guard;
- Method Runbook;
- role charter and launch-prompt templates;
- Process state;
- methodology roadmap;
- pattern evidence matrix;
- recovery guidance.

### Maturity

PAT-016 remains Candidate Pattern.

Additional cross-role transitions must test whether the contract improves zero-context startup and authority discipline without creating unnecessary administrative overhead.

### Cursor

M04 remains active. This work is additive bootstrap/runtime support and does not advance or reset the M04 cursor.

### Exact next Process action

Continue the remaining M04 generic client control-plane bootstrap kit artifacts.

## 2026-10-04 — Cross-role handoff authority firewall

### Trigger

Follow-up review of PAT-016 exposed a subtle risk: a durable handoff could itself become a backdoor authority channel if the sending role's recommendations were treated as instructions simply because they were written into durable state.

### Method rule

Handoffs now transfer context, not authority.

Material handoff content is classified as:

- authoritative fact;
- adopted decision / valid sponsor direction;
- recommendation / hypothesis;
- dependency / request;
- unknown / disputed.

The receiving role follows the real source authority for facts and adopted decisions. Recommendations and dependency requests remain non-binding.

Titles such as Chief, Executive, Stakeholder, or Lead do not create override rights.

### Conflict ladder

Cross-role disagreement now resolves in this order:

1. authoritative source;
2. owning domain / workstream;
3. valid human authority for genuine authority/adoption conflict;
4. ordinary non-material disagreement remains within the receiving role's charter.

This deliberately avoids both failure modes:

- one AI role overwriting another role's domain through a handoff; and
- unnecessary human bottlenecks for routine professional disagreement.

A generic human steward is not automatically the final authority; the client's authority model determines the correct human decision-maker.

### Maturity

MOBS-005 remains implemented.

PAT-016 remains Candidate Pattern and now requires field evidence involving real cross-domain disagreement, not merely successful context transfer.

### Cursor

M04 remains active and unchanged.

