# Changelog

## 2026-10-01

### Added

- Tenshodo Process consultancy-methodology foundation.
- Public/client confidentiality boundary.
- DEC-0001 Portable Method and Client Boundary.
- Method principles and engagement lifecycle.
- Client control-plane repository architecture.
- Pattern maturity model.
- Pattern evidence matrix with artifact-level source locators.
- Methodology runbook.
- Zero-context durability playbook.
- Organizational bootstrap playbook.
- AI role-incubation playbook.
- Change-impact/adoption playbook.
- Client CONTINUE_HERE and state templates.
- Portable role-conversation charter and decision-record template.
- Reusable role-conversation launch-prompt template with source-of-truth precedence, stale-prompt safeguards, execution-class boundaries, artifact-state limits, adoption authority, and durability requirements.
- Sanitized Tenshodo field notes.
- PROCESS_STATE.json and METHODOLOGY_ROADMAP.md.
- Foundation worklog.

### Changed

- Expanded the AI role-incubation playbook to define the standard launch protocol.
- Added role-conversation launch-prompt generation to the M04 client bootstrap kit.
- Registered the launch prompt as a standard methodology template in PROCESS_STATE.json.
- Expanded every active pattern with operating conditions, failure modes, applicability limits/counterexamples, falsifiers, artifact-level evidence, and portability gaps.
- Completed the M02 maturity calibration without promoting any pattern beyond the available evidence.
- Advanced the methodology cursor to M03; M04 is now dependency-ready.

## 2026-10-02

### Added

- Portable conversation-bootstrap protocol.
- Stable engagement-step registry with ordinal aliases (`Step 2` → `ENG-02`).
- One-line engagement quick-start instructions.
- Generic client `PROCESS_CONTEXT.json` template.
- `PROCESS_POINTER.json` template for non-control client repositories.

### Changed

- CONTINUE_HERE.md now routes engagement-step requests separately from methodology-development work.
- METHOD_RUNBOOK.md now defines engagement runtime and recovery behavior.
- README.md documents the one-line conversation launch experience.
- ENG-02 now resolves context/pointer files before reading large client repository state.
- M04 bootstrap-kit scope now includes deterministic multi-repository routing.

## 2026-10-03

### Added

- `playbooks/05-current-state-discovery.md` — governing Current-State Discovery SOP.
- `templates/DISCOVERY_INTAKE_CHECKLIST.md`.
- `templates/EXECUTIVE_SPONSOR_INTERVIEW.md`.
- `templates/CURRENT_STATE_CONFIDENCE_MAP.json`.
- `templates/CURRENT_STATE_DISCOVERY_ASSESSMENT.md`.
- `templates/DISCOVERY_OUTPUT_CONTRACT.md`.

### Changed

- Added the evidence-first discovery headline as Method Principle 16.
- Expanded Stage 1 of the engagement lifecycle into the standard evidence → process → inference → validation → baseline sequence.
- Formalized document-led, hybrid, and interview-led discovery modes.
- Formalized the evidence escalation ladder.
- Explicitly prohibited inferring consequential decision authority from title/activity alone.
- Completed M03 and advanced the methodology-development cursor to M04.

### Current state

M01, M02, and M03 are complete.

M04 — Build client control-plane bootstrap kit — is active.

No pattern is currently classified as Portable.

## 2026-10-03 — Role-routing guard and Next-Step Contract

### Added

- `docs/ROLE_ROUTING_GUARD.md`.
- Role-binding state model: `unbound`, `bound_correct`, `bound_wrong`.
- Mandatory wrong-role stop/handoff behavior.
- Mandatory end-of-batch Next-Step Contract.
- Role-binding requirements in `templates/ROLE_CONVERSATION_CHARTER.md`.
- Role-binding and self-handoff requirements in `templates/ROLE_CONVERSATION_LAUNCH_PROMPT.md`.

### Changed

- `PROCESS_CONTEXT.json` template now carries the role guard and next-step contract.
- Conversation bootstrap and method runbooks now require role-binding resolution before substantive work.
- Process runtime now registers the guard as standard M04 bootstrap prework.
- README now documents wrong-role protection and conversation self-handoff.

### Operator outcome

A user may send the generic Process command to the wrong role conversation. That conversation must not switch hats or perform the other role's work; it must identify the correct live role and tell the user exactly where to go next.


## 2026-10-03 — Parallel workstreams and commercialization module

### Added

- `docs/PARALLEL_WORKSTREAM_MODEL.md`.
- `templates/WORKSTREAM_REGISTRY.json`.
- `modules/commercialization/README.md`.
- `templates/COMMERCIALIZATION_BRAND_MARKET_FOUNDATION.md`.
- `templates/COMMERCIALIZATION_OFFER_ARCHITECTURE.md`.
- `templates/COMMERCIALIZATION_CLAIMS_REGISTER.md`.
- `templates/COMMERCIALIZATION_SALES_ENABLEMENT_HANDOFF.md`.

### Changed

- `PROCESS_CONTEXT.json` can now point to an optional client workstream registry.
- Conversation bootstrap now resolves role binding before workstream routing.
- Engagement lifecycle now allows parallel workstream activation when multiple independently executable bodies of work exist.
- M04 bootstrap scope now includes workstream routing and optional domain modules.
- Process runtime now exposes an explicit multi-workstream command pattern.
- README documents the optional-module model.

### Commercialization boundary

The Process module contains reusable method and templates only.

Client brand identity, decks, claims, pricing, customer evidence, market state, and sales execution remain client-specific.

## 2026-10-03 — Multi-environment discovery and methodology feedback loop

### Added

- provider-neutral Working-Plane Topology model;
- Environment Registry;
- Information Authority Register;
- Information Flow Register;
- optional Connected Discovery module;
- Connected Discovery Scope;
- Process Evidence Graph;
- terminology crosswalk template;
- Method Observation template and durable observation register;
- PAT-012 through PAT-015 as Candidate Patterns.

### Changed

- discovery now supports maturity-adaptive acquisition: process corpus, targeted validation, targeted connected read, or broader authorized connected read;
- current-state confidence provenance can identify environment/location, source lineage, evidence independence, and access scope;
- connector discovery is tenant/environment aware;
- PROCESS_CONTEXT can point to environment/authority/flow/discovery-scope registries without duplicating their content;
- 10XP is recorded as the human-layer shorthand for Tenshodo Process;
- substantive governed batches may signal methodology observations without adding a new Next-Step Contract routing state;
- methodology observations can be captured while M04 remains the active method cursor.

### Maturity boundary

These additions are durable method architecture but remain Candidate Patterns until field validation justifies promotion.

## 2026-10-04 — Durable cross-role handoff contract

### Trigger

A governed role transition demonstrated that correct successor-role routing and correct context transfer are separate control problems. The Role Routing Guard already defined where execution should go next, but the portable method did not define a generic artifact for the durable context that may cross the role boundary.

### Added

- `templates/ROLE_HANDOFF.md`.
- MOBS-005 — role transitions require explicit routing plus a durable cross-role context contract.
- PAT-016 — Durable cross-role handoff contract — Candidate Pattern.

### Changed

- `docs/ROLE_ROUTING_GUARD.md` now distinguishes routing from context transfer and calls for a Role Handoff Contract when material cross-role context exists.
- `METHOD_RUNBOOK.md` now defines the cross-role handoff method.
- `templates/ROLE_CONVERSATION_CHARTER.md` and `templates/ROLE_CONVERSATION_LAUNCH_PROMPT.md` now require durable handoff context when a successor role needs more than a simple task pointer.
- `PROCESS_STATE.json` registers the Role Handoff template as M04 prework/runtime support.
- `METHODOLOGY_ROADMAP.md` includes the durable cross-role handoff contract in M04.
- `patterns/EVIDENCE_MATRIX.md` includes PAT-016 evidence and portability gap.
- `CONTINUE_HERE.md` exposes the capability for zero-context methodology recovery.

### Boundary

The handoff is not a transcript, memory export, or new authority. It carries source pointers, durable shared facts, unresolved assumptions, dependencies, authority limits, and the receiving task. Live client state remains controlling.

M04 remains the active methodology cursor; no portability promotion occurred.

## 2026-10-04 — Cross-role handoff authority firewall

### Refined

PAT-016 and the Role Handoff Contract now distinguish **context transfer from authority transfer**.

A sending role may pass durable source pointers, facts, recommendations, dependencies, and open questions, but it may not use a handoff to override the receiving role's charter, supersede another role's governing source, or convert its own recommendation into an adopted instruction.

Role labels such as Chief, Executive, Stakeholder, or Lead do not confer cross-role override authority without a separate durable authority record.

### Disagreement resolution

Receiving roles now use this order:

1. resolve from declared authoritative sources;
2. route unresolved domain-owned questions to the owning role/workstream;
3. escalate genuine authority/adoption conflicts to the valid human authority for that decision class;
4. keep non-material professional disagreement within the receiving role's charter.

A generic human steward is not automatically the final decision authority. Stewardship may coordinate escalation, but decision authority remains separately governed.

### Updated

- `templates/ROLE_HANDOFF.md`
- `docs/ROLE_ROUTING_GUARD.md`
- `METHOD_RUNBOOK.md`
- `templates/ROLE_CONVERSATION_CHARTER.md`
- `templates/ROLE_CONVERSATION_LAUNCH_PROMPT.md`
- MOBS-005
- PAT-016
- `PROCESS_STATE.json`
- `patterns/EVIDENCE_MATRIX.md`
- `METHODOLOGY_ROADMAP.md`

M04 remains the active methodology cursor and PAT-016 remains Candidate Pattern.

