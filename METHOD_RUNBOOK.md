# Tenshodo Process — Methodology Runbook

## Purpose

This runbook governs how the consulting method itself evolves.

The repository should not become a scrapbook of clever ideas. It should preserve reusable patterns whose maturity can be explained and defended.

## Request routing

Before using the methodology-development cursor, determine whether the user is asking to:

- **develop Tenshodo Process itself**; or
- **execute a client engagement step**.

For client engagement-step requests, follow:

1. `engagement/STEP_REGISTRY.json`;
2. `docs/CONVERSATION_BOOTSTRAP_PROTOCOL.md`;
3. the client's `PROCESS_CONTEXT.json`;
4. the client's live durable state.

Do not resume PROCESS_STATE.json merely because this repository was opened.

For methodology-development work, use the startup sequence below.

## Methodology startup

1. Read CONTINUE_HERE.md.
2. Read PROCESS_STATE.json.
3. Read METHODOLOGY_ROADMAP.md.
4. Read patterns/PATTERN_REGISTRY.json.
5. Read patterns/EVIDENCE_MATRIX.md.
6. Read docs/PORTABILITY_AND_CONFIDENTIALITY.md.
7. Read the latest relevant field notes and worklog.

## Engagement runtime

Portable engagement steps use stable IDs.

The initial registry maps:

- Step 1 → ENG-01
- Step 2 → ENG-02
- Step 3 → ENG-03
- Step 4 → ENG-04
- Step 5 → ENG-05
- Step 6 → ENG-06

When a user says "check the process and execute Step 2", resolve the ordinal through the registry rather than relying on memory.

The client context packet is a pointer layer, not the authority. Live client state wins.

## Pattern capture workflow

When a live engagement reveals a potentially reusable lesson:

1. **Observe** — describe the problem and what happened.
2. **Sanitize** — remove client-specific/confidential details.
3. **Abstract** — identify the mechanism rather than copying the client's implementation.
4. **Register** — create/update a pattern ID.
5. **Evidence** — link sanitized case evidence.
6. **Bound** — record assumptions, conditions, failure modes, and counterexamples.
7. **Classify maturity** — observed / candidate_pattern / validated / portable / deprecated.
8. **Operationalize** — update a playbook/template only when evidence justifies it.
9. **Checkpoint** — update state, roadmap, worklog, and changelog.

## Promotion rules

### Observed → Candidate Pattern

Require:

- named problem;
- plausible generalized mechanism;
- reason the lesson might matter beyond one incident.

### Candidate Pattern → Validated

Require meaningful repeated use and evidence that the intended outcome occurred.

Repeated use in one company can validate a pattern internally.

### Validated → Portable

Require either:

- successful use in materially different organizational environments; or
- comparably strong evidence that the abstraction is not dependent on the originating client/domain/tool stack.

Default to **not portable** when uncertain.

## Client evidence handling

Never copy confidential client state into this repository.

Use abstract case IDs and sanitized descriptions.

Store detailed evidence in the client's authorized environment when it must remain private.

The public methodology may record that evidence exists without exposing it.

## Playbook changes

A playbook should answer:

- when to use the pattern;
- what problem it solves;
- prerequisites;
- step-by-step method;
- controls;
- failure/recovery behavior;
- definition of success;
- known conditions/limits.

Avoid enormous universal playbooks where smaller composable patterns work.

## Template changes

Templates are accelerators, not doctrine.

A template should expose:

- placeholders;
- authority assumptions;
- fields the consultant must verify;
- explicit unknowns rather than invented defaults.

## Recovery

If methodology work is interrupted:

- trust committed repository state;
- verify what files actually landed;
- do not credit an attempted write that cannot be verified;
- resume PROCESS_STATE.json current_task_id.

If an engagement launch is interrupted:

- trust the client repository;
- re-read PROCESS_CONTEXT.json and live client state;
- reconcile before resuming.

## Session end

Before ending substantive methodology work:

1. validate changed artifacts;
2. update pattern maturity/evidence where applicable;
3. update PROCESS_STATE.json;
4. update METHODOLOGY_ROADMAP.md if task status changed;
5. append worklog;
6. update CHANGELOG.md;
7. verify exact next action.
