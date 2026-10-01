# CONTINUE HERE — Tenshodo Process

This repository is the durable source for the Tenshodo consulting methodology.

A new consultant, employee, ChatGPT conversation, or agent should resume methodology work from repository state rather than reconstructing it from prior conversations.

## Startup order

Read:

1. PROCESS_STATE.json
2. METHODOLOGY_ROADMAP.md
3. METHOD_RUNBOOK.md
4. decisions/DEC-0001-portable-method-and-client-boundary.md
5. docs/CONSULTING_MODEL.md
6. docs/METHOD_PRINCIPLES.md
7. docs/PATTERN_MATURITY_MODEL.md
8. patterns/PATTERN_REGISTRY.json
9. patterns/EVIDENCE_MATRIX.md
10. docs/PORTABILITY_AND_CONFIDENTIALITY.md
11. latest relevant case-study notes, worklog, and CHANGELOG.md

Then read the playbook or template relevant to the active methodology task.

## Core rule

This repository contains **portable method**, not client operating state.

When learning from a live client or Tenshodo Exchange:

1. identify the observed lesson;
2. sanitize it;
3. record evidence without importing confidential data;
4. classify the pattern maturity honestly;
5. document conditions and failure modes;
6. update a reusable playbook or template only when justified.

## Current directive

Build a consultancy-grade transformation method that can be carried from organization to organization.

Do not prematurely call every Tenshodo design portable.

Repeated success inside one organization can validate a pattern internally, but portability requires evidence that the abstraction survives a materially different environment.

The active task is M02 — build the pattern evidence matrix and calibrate maturity.

## Checkpoint rule

After substantive methodology work:

- update PROCESS_STATE.json;
- update METHODOLOGY_ROADMAP.md if state changes;
- update the pattern registry and evidence matrix when evidence changes;
- append the methodology worklog;
- update CHANGELOG.md;
- commit an exact next action.

## Boundary

This repository is public.

Never copy private client or employer information into it.
