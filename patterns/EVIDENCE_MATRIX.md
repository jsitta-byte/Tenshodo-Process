# Pattern Evidence Matrix

This matrix is the human-readable companion to PATTERN_REGISTRY.json.

It records why current maturity labels are intentionally conservative.

| Pattern | Current maturity | Field evidence | What is demonstrated | What is not yet demonstrated |
|---|---|---|---|---|
| PAT-001 Zero-context resumability | Validated | CASE-TENSHODO-001 | Multiple interrupted/continued sessions can resume from durable state without restarting completed work | Use in a materially different company/domain |
| PAT-002 Bounded execution and checkpointing | Validated | CASE-TENSHODO-001 | Deterministic batches and remaining-work queues survive interruption and connector limits | Broad non-research departmental workflows |
| PAT-003 Working/control plane separation | Validated | CASE-TENSHODO-001, 002 | Collaborative working artifacts can coexist with Git-based durable control state when authority is explicit | Alternate stacks and different client cultures |
| PAT-004 No-dual-canonical rule | Validated | CASE-TENSHODO-001 | Declared working authority plus generated checkpoint exports reduces ambiguity during recovery | Cross-company replication |
| PAT-005 Live-source revalidation | Validated | CASE-TENSHODO-001 | Upstream source changes can be reconciled before earlier classifications are credited | Non-code operational sources such as CRM/ERP/HRIS |
| PAT-006 Target accountability vs current execution | Candidate Pattern | CASE-TENSHODO-002 | The distinction resolves a conceptual governance deadlock | Sustained operating use |
| PAT-007 Organizational bootstrap layer | Candidate Pattern | CASE-TENSHODO-002 | A transition layer provides a path when target roles do not exist | Repeated execution and successful retirement of bootstrap authority |
| PAT-008 AI role incubation | Candidate Pattern | CASE-TENSHODO-002 | A governed design exists for building a function before a human steward is selected | Completed incubation → human takeover cycle |
| PAT-009 Proposal/adoption separation | Candidate Pattern | CASE-TENSHODO-002 | Explicit decision-state separation addresses false-authority risk | Repeated operational adoption cycles |
| PAT-010 Dependency-aware process change | Candidate Pattern | CASE-TENSHODO-002 | Lifecycle and candidate-blast-radius model are defined | Full dependency graph and real cross-functional change cycle |
| PAT-011 Separate truth dimensions | Candidate Pattern | CASE-TENSHODO-001 | Independent evidence dimensions prevented domain-specific truth collapse | Generalized examples across business functions |

## Current conclusion

The durability engine has meaningful internal validation.

The organizational/AI management patterns are promising but early.

No current pattern has enough cross-environment evidence to be labeled Portable.
