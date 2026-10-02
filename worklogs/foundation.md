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

### Observation

The first AI-incubated management role was launched using a carefully written opening ChatGPT command that pointed the conversation back to durable GitHub state.

### Established

- Created templates/ROLE_CONVERSATION_LAUNCH_PROMPT.md.
- Established that the launch prompt is an ignition key, not the source of truth.
- Required live durable state and declared authoritative systems to override stale prompt content.
- Added stale-prompt checks and explicit authority boundaries.
- Added the launch protocol to the AI role-incubation playbook.
- Registered the template as M04 client-bootstrap prework.

## 2026-10-01 — M02 evidence calibration completed

### Objective

Prevent the emerging consultancy method from turning Tenshodo-specific enthusiasm into unsupported doctrine.

### Work performed

For every active pattern, added:

- operating conditions;
- failure modes;
- counterexample or applicability limit;
- falsifier;
- artifact-level sanitized evidence locators;
- explicit portability gap.

### Evidence sources

The durability patterns were grounded in current durable artifacts from jsitta-byte/Tenshodo-Exchange.

The organizational/AI patterns were grounded in current durable decisions, models, and state from jsitta-byte/Tenshodo-Exchange-Management.

### Maturity decisions

Remain Validated:

- PAT-001 Zero-context resumability
- PAT-002 Bounded execution and checkpointing
- PAT-003 Working/control plane separation
- PAT-004 No-dual-canonical rule
- PAT-005 Live-source revalidation

Remain Candidate Pattern:

- PAT-006 Target accountability vs current execution
- PAT-007 Organizational bootstrap
- PAT-008 AI role incubation
- PAT-009 Proposal/adoption separation
- PAT-010 Dependency-aware process change
- PAT-011 Separate truth dimensions

No pattern was promoted to Portable.

### Completion

M02 definition of done is satisfied.

### Exact next action

Execute M03: build the consultancy kickoff and discovery kit so the team can enter a new client, discover current authority/work systems/pain points/AI readiness/confidentiality constraints, and produce a clean discovery package for M04 client control-plane bootstrap.


## 2026-10-02 — Process-driven conversation bootstrap established

### Problem

The first role conversation could be launched safely, but doing so still required the human operator to paste a long, carefully constructed prompt.

That is not sufficiently repeatable for a consultancy operating across many clients and functions.

### Decision

Move substantive launch context out of the human prompt.

Use a two-layer resolver:

- Tenshodo Process contains the portable engagement-step protocol.
- Each client control plane contains a small `PROCESS_CONTEXT.json` pointer packet.

### Established

- `docs/CONVERSATION_BOOTSTRAP_PROTOCOL.md`
- `engagement/STEP_REGISTRY.json`
- `engagement/QUICK_START.md`
- `templates/PROCESS_CONTEXT.json`
- request routing in `CONTINUE_HERE.md`
- engagement runtime rules in `METHOD_RUNBOOK.md`

### Stable step model

- ENG-01 — establish engagement context
- ENG-02 — resolve and launch current work conversation
- ENG-03 — execute bounded work and checkpoint
- ENG-04 — route decisions/adoption
- ENG-05 — transfer/rotate stewardship
- ENG-06 — close/transition engagement

Human-friendly ordinals map to stable IDs. Existing IDs should not be renumbered after publication.

### Intended operator experience

A configured client should normally require only:

`Check Tenshodo-Process and execute Engagement Step 2 for <client>.`

Or:

`Check Tenshodo-Process and execute the current engagement step for <client>.`

### Boundary

The public Process repository defines how context is resolved; live client context remains in the client repository.

### Next methodology action

Continue M03 — build the consultancy kickoff and discovery kit.


## 2026-10-02 — Live Step-2 launch exposed repository ambiguity

### Observation

A fresh conversation received the intended one-line command:

`Check Tenshodo-Process and execute the current engagement step for Tenshodo Exchange.`

It correctly read the Process bootstrap layer, but initially treated `jsitta-byte/Tenshodo-Exchange` as a candidate client control plane because the repository name matched the client name.

That specialized project repository did not contain `PROCESS_CONTEXT.json`. The conversation inferred that `Tenshodo-Exchange-Management` was likely the control plane, but the run timed out while validating the redirect.

### Lesson

A multi-repository client needs deterministic repository routing before the resolver reads substantive project state.

### Change

- Added a generic `PROCESS_POINTER.json` template.
- Added aliases and `repository_role` to `PROCESS_CONTEXT.json`.
- ENG-02 now checks routing files before large plans/state.
- Non-control client repositories may point directly to the engagement control plane.
- Added the pointer pattern to M04 bootstrap prework.

### Expected result

A new conversation should resolve:

named client → small routing file → client control repository → PROCESS_CONTEXT → live client state

without exploratory project reads.
