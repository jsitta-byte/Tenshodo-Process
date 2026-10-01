# CONTINUE HERE — Tenshodo Process

This repository is the durable source for the Tenshodo consulting methodology.

A new consultant, employee, ChatGPT conversation, or agent should resume methodology work from repository state rather than reconstructing it from prior conversations.

## Startup order

Read:

1. PROCESS_STATE.json
2. METHODOLOGY_ROADMAP.md
3. docs/CONSULTING_MODEL.md
4. docs/METHOD_PRINCIPLES.md
5. docs/PATTERN_MATURITY_MODEL.md
6. patterns/PATTERN_REGISTRY.json
7. docs/PORTABILITY_AND_CONFIDENTIALITY.md
8. latest relevant case-study notes, worklog, and CHANGELOG.md

Then read the playbook or template relevant to the active methodology task.

## Core rule

This repository contains **portable method**, not client operating state.

When learning from a live client or Tenshodo Exchange:

1. identify the observed lesson;
2. sanitize it;
3. record evidence without importing confidential data;
4. classify the pattern maturity honestly;
5. update a reusable playbook or template only when justified;
6. preserve conditions and failure modes.

## Current directive

Build a consultancy-grade transformation method that can be carried from organization to organization.

Do not prematurely call every Tenshodo design portable.

Repeated success inside one organization can validate a pattern internally, but portability requires evidence that the abstraction survives a materially different environment.

## Checkpoint rule

After substantive methodology work:

- update PROCESS_STATE.json;
- update METHODOLOGY_ROADMAP.md if state changes;
- update the pattern registry when evidence changes maturity;
- append the methodology worklog;
- update CHANGELOG.md;
- commit an exact next action.

## Boundary

Never copy private client or employer information into this public methodology repository.
