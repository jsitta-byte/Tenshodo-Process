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
