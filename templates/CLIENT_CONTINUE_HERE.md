# CONTINUE HERE — <Client / Program>

This repository is the durable control plane for <scope>.

Do not reconstruct work from conversation history.

## Read first

1. COMPANY_STATE.json
2. TRANSFORMATION_PLAN.md
3. OPERATING_RUNBOOK.md
4. <authority/source model>
5. latest relevant decision record and worklog

## Before executing

Verify:

- current task;
- current executor;
- target owner;
- live external source state where relevant;
- adoption authority;
- exact next action.

## Core rule

Only validated, durably checkpointed work counts as complete.

## Session end

Update durable state, worklog, relevant decisions, and exact next action before ending substantive work.
