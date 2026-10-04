# Pattern Evidence Matrix

This matrix is the human-readable companion to PATTERN_REGISTRY.json.

The machine-readable registry contains the full conditions, failure modes, limits, falsifiers, and artifact-level evidence locators.

## Calibration summary

| Pattern | Maturity | Evidence | Operating conditions | Primary failure mode | Portability gap |
|---|---|---|---|---|---|
| PAT-001 Zero-context resumability | Validated | CASE-TENSHODO-001 | Durable state is current, accessible, and includes exact next action | Critical context remains only in chat or stale handoff | Different company/domain |
| PAT-002 Bounded execution and checkpointing | Validated | CASE-TENSHODO-001 | Work can be partitioned and validated deterministically | Partial attempts counted as complete; next boundary omitted | Non-research departmental workflows |
| PAT-003 Working/control plane separation | Validated | CASE-TENSHODO-001, 002 | Authority per information class is explicit | Both planes become editable authorities | Alternate stacks/cultures |
| PAT-004 No-dual-canonical rule | Validated | CASE-TENSHODO-001 | One authority + declared replicas/cutover | Users edit source and replica independently | Cross-company replication |
| PAT-005 Live-source revalidation | Validated | CASE-TENSHODO-001 | Source identity/state can be detected and checkpointed | Revalidation ignores material relevant changes | CRM/ERP/HRIS-style sources |
| PAT-006 Target vs current authority | Candidate Pattern | CASE-TENSHODO-002 | Transitional organization with identifiable current authority | Target title is mistaken for present authority | Sustained use + external validation |
| PAT-007 Organizational bootstrap | Candidate Pattern | CASE-TENSHODO-002 | Real bootstrap deadlock + sponsor + exit condition | Temporary authority becomes permanent | Repeated activation and clean retirement |
| PAT-008 AI role incubation | Candidate Pattern | CASE-TENSHODO-002 | Non-binding build work + durable charter + separate human authority | AI role mistaken for executive / knowledge trapped in chat | Completed human takeover |
| PAT-009 Proposal/adoption separation | Candidate Pattern | CASE-TENSHODO-002 | Adoption authority can be named and status can be enforced | Proposed work is treated as binding | Repeated adoption cycles |
| PAT-010 Dependency-aware process change | Candidate Pattern | CASE-TENSHODO-002 | Useful dependency data + owners decide scope | Impact map becomes automatic scope or stale bureaucracy | Full change cycle with graph |
| PAT-011 Separate truth dimensions | Candidate Pattern | CASE-TENSHODO-001 | Distinct evidence/time-sensitive truth questions exist | Complexity without decision value | Business-domain examples |

## Artifact-level evidence locators

### CASE-TENSHODO-001 — Durable long-running project recovery

- `jsitta-byte/Tenshodo-Exchange/CONTINUE_HERE.md@451d1eaf14ab6cc62874c1887792c83b373dd89e`
- `jsitta-byte/Tenshodo-Exchange/PROJECT_STATE.json@308e7ea0a1dd9002d1a9a73fa7c89c94b400a0eb`
- `jsitta-byte/Tenshodo-Exchange/CHATGPT_RUNBOOK.md@10f64e612f176ba76aaf58707658816eb18740c4`
- `jsitta-byte/Tenshodo-Exchange/PROJECT_PLAN.md@2acc64947857ee803a755f88211e0ed2c1dee2fd`

These artifacts demonstrate a repeated operating pattern: work is selected from durable state, live source/work surfaces are revalidated, bounded batches are checkpointed, and interrupted work is reconciled rather than trusted from chat memory.

### CASE-TENSHODO-002 — Management-system bootstrap

- `jsitta-byte/Tenshodo-Exchange-Management/decisions/DEC-0002-organizational-bootstrap-authority-and-transitional-stewardship.md@963e85e364fdb4e7567b9ec918ba2f81e0343d28`
- `jsitta-byte/Tenshodo-Exchange-Management/decisions/DEC-0003-ai-role-incubation-and-human-handoff.md@c677525d1ac743b26c7001032637e34e1649ac95`
- `jsitta-byte/Tenshodo-Exchange-Management/docs/AI_ROLE_INCUBATION.md@e29f8f5d776004a4c2f447082a95d2a7b100c2fb`
- `jsitta-byte/Tenshodo-Exchange-Management/docs/PROCESS_CHANGE_SYSTEM.md@b7db95883116cb14f28abacca73d156af5937b24`
- `jsitta-byte/Tenshodo-Exchange-Management/COMPANY_STATE.json@c98d9a5ee7674f1ed5ff6af89d553a1702d13f3c`

These artifacts demonstrate that the newer governance and AI patterns are explicitly designed and activated in durable state, but most have not yet completed enough real operating cycles to justify Validated status.

## Maturity decisions after M02 calibration

### Remain Validated

PAT-001 through PAT-005 remain **Validated** because they have repeated operating evidence within the first field laboratory, including interruption/recovery behavior.

They are not promoted to Portable because materially different organizational environments have not yet tested them.

### Remain Candidate Pattern

PAT-006 through PAT-011 remain **Candidate Pattern**.

The calibration pass found no evidence strong enough to justify promotion.

In particular:

- PAT-007 still lacks a completed bootstrap → retirement cycle.
- PAT-008 still lacks a completed AI incubation → human takeover cycle.
- PAT-009 still lacks repeated real adoption cycles.
- PAT-010 still lacks a fully operating dependency graph and end-to-end cross-functional change.
- PAT-011 lacks business-domain examples outside the original project truth model.

## M02 conclusion

Every active pattern now has:

- explicit field evidence;
- artifact-level evidence locators;
- operating conditions;
- failure modes;
- a counterexample or applicability limit;
- a falsifier;
- a stated portability gap;
- a defensible maturity decision.

This satisfies the M02 evidence-calibration definition of done.

No pattern is currently Portable.

## Additive candidate patterns from multi-environment discovery architecture

| Pattern | Maturity | Evidence | Operating conditions | Primary failure mode | Portability gap |
|---|---|---|---|---|---|
| PAT-012 Multi-environment working-plane topology | Candidate Pattern | CASE-TENSHODO-002 + sanitized method capture | Material environment/tenant boundaries exist and can be identified | Provider name still substitutes for environment identity or topology becomes needless bureaucracy | External multi-tenant/multi-provider use |
| PAT-013 Maturity-adaptive connected discovery | Candidate Pattern | Sanitized method capture | Access scope can be governed and discovery maturity can be assessed | Broad access by default; observation mistaken for authority; wrong-tenant evidence | Comparative discovery across different maturity levels |
| PAT-014 Semantic terminology crosswalk before renaming | Candidate Pattern | Sanitized method capture | Similar concepts exist under different labels | Labels assumed equivalent or source vocabulary overwritten too early | Real cross-team/cross-company integration |
| PAT-015 Parallel methodology observation queue | Candidate Pattern | Sanitized method capture | Method Steward can triage and confidentiality boundary is preserved | Queue becomes backlog or hijacks active cursor | Repeated field-to-method cycles |
| PAT-016 Durable cross-role handoff with authority-preserving conflict resolution | Candidate Pattern | Sanitized method capture | Material governed work crosses roles; source/domain/adoption authority can be distinguished | Handoff becomes transcript or authority channel; routine disagreement is over-escalated; genuine authority conflicts are under-escalated | Repeated cross-role transitions with real disagreement across different functions and organizations |

### PAT-012 evidence

- `jsitta-byte/Tenshodo-Exchange-Management/decisions/DEC-0004-ten-ex-operating-architecture-correction.md@6bf310e34d37a31bf46e57d0401902be8c30f5b7`
- `jsitta-byte/Tenshodo-Process/docs/WORKING_PLANE_TOPOLOGY.md@eb0b123a76c60a11885803c4640cceb109a84f7e`
- `jsitta-byte/Tenshodo-Process/methodology/METHOD_OBSERVATION_REGISTER.json@9a3adb5a484ee8598c3b9a5b9ef5c010dc863b0f`

### PAT-013 evidence

- `jsitta-byte/Tenshodo-Process/modules/connected-discovery/README.md@f1bbaa95e799a3922c64e53bcd955aa6e82b3ba5`
- `jsitta-byte/Tenshodo-Process/methodology/METHOD_OBSERVATION_REGISTER.json@9a3adb5a484ee8598c3b9a5b9ef5c010dc863b0f`

### PAT-014 evidence

- `jsitta-byte/Tenshodo-Process/templates/TERMINOLOGY_CROSSWALK.md@f1bbaa95e799a3922c64e53bcd955aa6e82b3ba5`
- `jsitta-byte/Tenshodo-Process/methodology/METHOD_OBSERVATION_REGISTER.json@9a3adb5a484ee8598c3b9a5b9ef5c010dc863b0f`

### PAT-015 evidence

- `jsitta-byte/Tenshodo-Process/templates/METHOD_OBSERVATION.md@9a3adb5a484ee8598c3b9a5b9ef5c010dc863b0f`
- `jsitta-byte/Tenshodo-Process/METHOD_RUNBOOK.md@9a3adb5a484ee8598c3b9a5b9ef5c010dc863b0f`

### PAT-016 evidence

- `jsitta-byte/Tenshodo-Process/templates/ROLE_HANDOFF.md@7ec4764679d86ef8f383b95412991edeccb92555`
- `jsitta-byte/Tenshodo-Process/docs/ROLE_ROUTING_GUARD.md@92dff1b011ca1ea026ca2cdff9a4dcf8d8820fda`
- `jsitta-byte/Tenshodo-Process/methodology/METHOD_OBSERVATION_REGISTER.json@6403c3a7760644db837f76554c1ab5796c19cb40`

These patterns are intentionally not promoted beyond Candidate Pattern. The architecture is now durable; portability remains to be earned through field evidence. PAT-016 specifically requires repeated zero-context role transitions, including genuine cross-domain disagreement, showing that the handoff contract reduces reconstruction and authority leakage while distinguishing routine professional disagreement from human-required authority/adoption conflicts without creating unnecessary process overhead.
