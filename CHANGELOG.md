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

### Current state

M01 and M02 are complete.

M03 — Build consultancy engagement kickoff and discovery kit — is active.

M04 — Build client control-plane bootstrap kit — is ready.

No pattern is currently classified as portable.


## 2026-10-02

### Added

- Portable conversation-bootstrap protocol.
- Stable engagement-step registry with ordinal aliases (`Step 2` → `ENG-02`).
- One-line engagement quick-start instructions.
- Generic client `PROCESS_CONTEXT.json` template.

### Changed

- CONTINUE_HERE.md now routes engagement-step requests separately from methodology-development work.
- METHOD_RUNBOOK.md now defines engagement runtime and recovery behavior.
- README.md documents the one-line conversation launch experience.
- PROCESS_STATE.json now registers engagement runtime artifacts and PROCESS_CONTEXT as standard M04 prework.
- M04 bootstrap-kit scope now requires a client context packet and step resolver.

### Current state

The repeatable conversation launch path is now:

short operator command → portable ENG step → client PROCESS_CONTEXT.json → live client state → role START_HERE / charter → bounded execution.

M03 remains the active methodology-development task.
