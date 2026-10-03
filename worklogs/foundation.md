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
