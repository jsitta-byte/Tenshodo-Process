# CONTINUE HERE — Tenshodo Process

This repository is the durable source for the Tenshodo consulting methodology **and the portable resolver for engagement-step launch requests**.

A new consultant, employee, ChatGPT conversation, or agent should not reconstruct work from prior chat history.

## First: route the request

Before following the methodology-development cursor, determine which mode the user requested.

### Engagement-step mode

If the user says something like:

- "check the process for Step 2";
- "execute Engagement Step 2 for <client>";
- "resume the current engagement step for <client>";
- "follow ENG-02";

then **do not automatically resume PROCESS_STATE.json current_task_id**.

Instead:

1. read `engagement/STEP_REGISTRY.json`;
2. read `docs/CONVERSATION_BOOTSTRAP_PROTOCOL.md`;
3. resolve the requested ordinal or stable ENG-ID;
4. identify the client control-plane repository;
5. read that client's `PROCESS_CONTEXT.json`;
6. reconcile the packet against live client state;
7. execute the engagement step under the client authority model.

The portable process defines how to launch. The client repository defines what is live.

### Methodology-development mode

If the user asks to develop, improve, document, or continue **Tenshodo Process itself**, use the methodology startup below and resume PROCESS_STATE.json current_task_id.

## Methodology startup order

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
11. methodology/METHOD_OBSERVATION_REGISTER.json
12. latest relevant case-study notes, worklog, and CHANGELOG.md

Then read the playbook or template relevant to the active methodology task.

## Core rule

This repository contains **portable method**, not client operating state.

When learning from a live client:

1. capture the reusable lesson durably before relying on memory;
2. keep client-private detail in the client environment;
3. sanitize the method observation;
4. register/triage it without hijacking the active methodology cursor;
5. record evidence without importing confidential data;
6. classify pattern maturity honestly;
7. document conditions and failure modes;
8. update a reusable playbook or template only when justified.

## Current methodology directive

The active methodology-development task is **M04 — Build client control-plane bootstrap kit**.

M03 remains complete. Additive discovery capabilities now include multi-environment working-plane topology, optional Connected Discovery, process-corpus shortcuts, Process Evidence Graphs, tenant-aware provenance, and terminology crosswalks.

Reusable lessons discovered during client work are captured in `methodology/METHOD_OBSERVATION_REGISTER.json` without changing the active M04 cursor merely because a new observation exists.

This cursor is irrelevant when the user's request is an engagement-step launch.

## Checkpoint rule

After substantive methodology work:

- update PROCESS_STATE.json;
- update METHODOLOGY_ROADMAP.md if state changes;
- update the Method Observation register when observations are captured/triaged;
- update the pattern registry and evidence matrix when evidence changes;
- append the methodology worklog;
- update CHANGELOG.md;
- commit an exact next action.

## Boundary

This repository is public.

Never copy private client or employer information into it.
