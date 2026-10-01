# Tenshodo Field Notes — Sanitized

These notes preserve the origins of the methodology without importing private operational data.

## CASE-TENSHODO-001 — Durable long-running project recovery

### Situation

A complex research/data project required hundreds of source files to be reviewed across many ChatGPT sessions and multiple external systems.

The work repeatedly encountered:

- conversation-length limits;
- connector retries;
- partial batches;
- changing upstream source state;
- working data outside GitHub.

### Intervention

The project introduced:

- machine-readable current-task state;
- human-readable plan;
- zero-context handoff;
- operating runbook;
- deterministic source ledgers;
- remaining-work queues;
- bounded batches;
- checkpoint after each batch;
- live source commit/tree revalidation;
- explicit authority separation between working artifacts, Git checkpoints, upstream source evidence, and time-sensitive evidence.

### Observed result

New sessions could resume from the durable cursor rather than repeating completed batches.

Interrupted work could be reconciled against the live working plane and deterministic source inventory.

### Patterns supported

- PAT-001 Zero-context resumability
- PAT-002 Bounded execution and checkpointing
- PAT-003 Working/control plane separation
- PAT-004 No-dual-canonical rule
- PAT-005 Live-source revalidation
- PAT-011 Separate truth dimensions

### Limit

This evidence comes from one specialized project environment.

## CASE-TENSHODO-002 — Management-system bootstrap

### Situation

A company-wide operating-system concept introduced target executive roles and attempted to route management-system work to them.

The model then deadlocked conceptually because:

- the target roles were not actually staffed;
- creating a workforce map appeared to require a People executive who did not yet exist;
- assigning prompt pilots required understanding the workforce first.

### Intervention

The management design introduced:

- target accountability separate from current execution;
- organizational bootstrap authority;
- temporary stewardship;
- AI role conversations that can incubate functions;
- explicit distinction between proposed work and adopted decisions;
- future human takeover from durable role state;
- candidate cross-functional impact maps rather than automatic change scope.

### Current status

These mechanisms have been designed and are entering field use.

They are not yet validated to the same level as the flagship durability patterns.

### Patterns supported

- PAT-006 Target vs current authority
- PAT-007 Organizational bootstrap
- PAT-008 AI role incubation
- PAT-009 Proposal/adoption separation
- PAT-010 Dependency-aware process change
