# Playbook 01 — Zero-Context Durability

## Use when

Work spans multiple sessions, people, systems, agents, or long time periods.

## Goal

A qualified successor can resume safely without reconstructing history from the previous operator.

## Minimum implementation

Create:

- machine-readable state;
- human-readable plan;
- operating runbook;
- zero-context handoff;
- append-oriented worklog;
- changelog;
- exact next action.

## State-file minimum

Record:

- current phase;
- current task;
- dependencies;
- completion status;
- authoritative working artifacts;
- source refs;
- invariants;
- counters/progress where useful;
- exact next action.

## Session startup

1. Read durable handoff.
2. Read state.
3. Read plan/runbook.
4. Revalidate live sources when they may have changed.
5. Reconcile discrepancies.
6. Resume only validated work.

## Session end

1. Validate completed work.
2. Update state.
3. Update plan if material.
4. Append worklog.
5. Update changelog.
6. Commit/checkpoint.
7. Verify exact next action is sufficient for a newcomer.

## Failure test

Ask another qualified operator with zero chat context to resume.

If they must ask "What were you doing?" the system failed.
