# Client Engagement Lifecycle

This lifecycle is a starting architecture, not an inflexible sequence.

## Stage 0 — Mandate and boundary

Establish:

- executive sponsor;
- engagement scope;
- access boundaries;
- confidentiality;
- adoption authority;
- consultant authority;
- prohibited actions;
- working-plane constraints;
- control-plane location.

Do not begin by redesigning the org chart.

## Stage 1 — Current-state discovery

Use the governing sequence:

**Evidence intake → current-process discovery → provisional inference → targeted validation → current-state baseline → transformation**

See `playbooks/05-current-state-discovery.md`.

### 1. Evidence intake

Collect or connect what already exists before asking people to recreate it:

- workforce / HR records;
- org charts;
- job descriptions;
- process material;
- authority/RACI records;
- system inventories;
- repositories;
- recurring reports;
- policy and approval records;
- current AI/automation evidence.

Do not ask the client to clean the evidence first.

### 2. Choose discovery mode

Classify the engagement as:

- document-led;
- hybrid;
- interview-led.

The methodology stays the same; the cost mix changes.

### 3. Discover current work

Establish enough of the actual recurring work to understand:

- people and responsibilities;
- triggers and outputs;
- systems/data;
- approvals;
- decisions;
- handoffs;
- pain points;
- workarounds;
- current AI use.

### 4. Infer only the gaps

Use provisional inference when authoritative/documentary/observed evidence does not cheaply answer the question.

Every inferred field must preserve provenance, confidence, rationale, and validation need.

Do not infer consequential decision authority from title or activity alone.

### 5. Validate selectively

Spend employee/manager/consultant time on:

- high-consequence ambiguity;
- conflicting evidence;
- cross-functional processes;
- undocumented authority;
- transformation-critical unknowns.

### 6. Establish the baseline

Create a Current-State Confidence Map that separates:

- authoritative;
- attested;
- observed;
- inferred;
- unknown;
- disputed.

Record unknowns instead of guessing.

Discovery ends when the organization is legible enough to route work and choose a safe transformation pilot—not when every field is perfect.

## Stage 2 — Durable control-plane bootstrap

Create the minimum structure required for resumable transformation:

- CONTINUE_HERE;
- machine-readable state;
- human-readable plan;
- runbook;
- decision records;
- worklog;
- change log;
- authority/source model;
- process context / routing where applicable.

Do not build the perfect enterprise ontology first.

## Stage 3 — Authority and truth mapping

For material information and decisions, determine:

- authoritative system;
- current decision authority;
- target accountability;
- evidence requirements;
- transition state.

Resolve dual-canonical risks.

## Stage 4 — Select a high-value pilot

Choose work where durability creates visible value.

Good pilots often have:

- repeated interruption;
- multiple tools;
- many dependencies;
- expensive context loss;
- recurring handoffs;
- material need for provenance.

Prove the durability engine before forcing it company-wide.

## Stage 5 — Organizational bootstrap

Where target roles are missing:

- use temporary stewardship;
- activate role conversations where useful;
- preserve authority boundaries;
- build the function;
- learn the actual requirements of the human role.

## Parallel-workstream activation

The engagement may remain single-cursor through early bootstrap.

Introduce parallel workstreams only when at least two durable bodies of work can proceed with distinct executors or independently useful checkpoints.

When that threshold is met:

- create a client workstream registry;
- keep one declared executor per workstream task;
- preserve role-conversation binding;
- record cross-workstream dependencies explicitly;
- keep one engagement control plane rather than creating competing canonical repositories.

See `docs/PARALLEL_WORKSTREAM_MODEL.md`.

Optional domain modules may be activated as workstreams when real work exists. For example, `modules/commercialization/` provides a commercialization spine for brand, offer, claims, marketing, and sales-enablement work without making commercialization mandatory for every engagement.

## Stage 6 — Process and dependency mapping

Model material:

- capabilities;
- processes;
- products/services;
- systems;
- data;
- controls;
- roles;
- documents;
- agents;
- vendors;
- metrics.

Build enough graph structure to support impact analysis.

## Stage 7 — Governed improvement loop

Establish:

suggest → triage → impact map → decision → plan → implement → validate → adopt → observe.

Keep candidate blast radius separate from approved scope.

## Stage 8 — Domain rollout

Extend durability patterns to areas such as:

- finance;
- sales;
- marketing;
- product;
- customer;
- people;
- technology;
- data/AI;
- legal/risk;
- security.

Do not assume every domain needs identical artifacts.

## Stage 9 — Human stewardship transfer

Transfer incubated functions to appropriate client employees as understanding and capacity mature.

Make delegation explicit.

Preserve the AI role as copilot, analyst, reviewer, or retire it.

## Stage 10 — Continuous operating review

Monitor:

- stale state;
- orphaned tasks;
- missing owners;
- failed checkpoints;
- conflicting authorities;
- process drift;
- outdated prompts/agents;
- unresolved dependency impacts.

The goal is not to finish documentation.

The goal is to create an organization that can safely keep changing.
