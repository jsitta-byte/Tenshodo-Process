# Current-State Discovery SOP

## Governing principle

> **Do not interview people for facts the organization can already prove. Do not infer facts the organization can cheaply confirm. Do not redesign the organization until you understand enough of the work and authority that actually exist.**

This SOP governs the discovery phase of a Tenshodo Process consulting engagement.

The purpose is not to create a perfect organizational model before work begins.

The purpose is to establish a sufficiently trustworthy current-state baseline so transformation can proceed without guessing.

## Standard sequence

**Evidence intake → current-process discovery → provisional inference → targeted validation → current-state baseline → transformation**

Do not reverse this sequence by:

- inferring detailed responsibilities before checking available evidence;
- redesigning processes before understanding the work that currently exists;
- interviewing everyone when authoritative records already answer the question;
- treating job titles as proof of decision authority;
- treating inferred profiles as adopted fact.

## Discovery modes

Every engagement should declare one discovery mode after initial intake.

### Document-led

Use when the client has strong, current records such as:

- HRIS roster;
- org chart;
- job descriptions;
- process library;
- RACI / authority matrix;
- system inventory;
- access records;
- policy repository;
- project/workflow evidence.

Consulting effort focuses on:

- reconciling sources;
- identifying drift between documented and actual work;
- filling exceptions;
- validating consequential ambiguities.

### Hybrid

Use when useful records exist but operating reality is incomplete or inconsistent.

Consulting effort combines:

- artifact ingestion;
- observed operational evidence;
- provisional inference;
- targeted employee/manager confirmation.

This is expected to be the most common mode.

### Interview-led

Use when the organization has little trustworthy documentation.

Consultants and AI should still prepare hypotheses from available evidence before interviews.

The objective is to ask:

> Is this an accurate description of how the work happens?

rather than beginning every conversation with:

> What do you do here?

## Evidence escalation ladder

For each required field, use the least expensive source capable of reaching the required confidence.

Preferred order:

1. authoritative business system;
2. controlled/documented record;
3. observed operational evidence;
4. AI / consultant inference;
5. asynchronous employee confirmation;
6. manager / accountable-owner confirmation;
7. consultant interview or workshop.

Move to a more expensive method only when the cheaper source is insufficient.

### Important exception — authority

Do not infer consequential decision authority from title, activity, seniority, or system usage alone.

Decision authority should be:

- directly documented;
- attested by a valid authority;
- or recorded as unknown / needs_attestation.

## Discovery dimensions

The current-state baseline should cover enough of these dimensions to support transformation:

### People

- current workforce membership;
- titles / descriptive positions;
- recurring responsibilities;
- observed work;
- subject-matter expertise;
- systems used;
- capacity;
- exclusions / known boundaries;
- current decision authority where proven.

### Processes

- recurring workflows;
- triggers;
- inputs;
- outputs;
- handoffs;
- approvals;
- exceptions;
- rework;
- failure points;
- workarounds;
- timing / cadence.

### Systems and information

- systems of record;
- working planes;
- shadow systems;
- spreadsheets;
- repositories;
- integrations;
- access patterns;
- duplicate truths;
- high-friction handoffs.

### Authority and governance

- current decision rights;
- escalation paths;
- policy ownership;
- adoption authority;
- material approval thresholds;
- unresolved ambiguity.

### AI / automation

- current AI and agent use;
- prompts or workflows in production;
- sensitive-data exposure;
- automation authority;
- validation controls;
- human-review expectations;
- failure / rollback handling.

### Pain and opportunity

- repeated interruption;
- duplicated entry;
- missing ownership;
- stale state;
- coordination failures;
- undocumented dependencies;
- slow approvals;
- low-value manual work;
- high context-loss work;
- opportunities for durable workflow or automation.

## Field-level evidence states

Every material current-state field should use one of these evidence states:

### authoritative

Directly supported by the currently declared system of record or adopted control artifact.

### attested

Confirmed by a person who has valid knowledge/authority to attest the fact.

### observed

Supported by direct operational evidence, but not formally declared authoritative.

### inferred

Reasonable provisional conclusion from available evidence.

Inference must include:

- provenance;
- confidence;
- rationale;
- validation requirement.

### unknown

No sufficient evidence exists.

### disputed

Material sources or people conflict.

Do not force disputed data into a false single truth.

## Confidence

Confidence is field-level, not person-level.

Recommended labels:

- high;
- medium;
- low;
- not_applicable.

Example:

A person may have:

- GitHub usage — observed / high;
- technical-analysis responsibility — inferred / medium;
- customer-facing role — unknown;
- spending authority — needs attestation / not inferred.

## Process-first rule

Detailed role inference should normally occur **after enough current-process discovery exists to provide evidence about actual work**.

This does not mean waiting to collect basic people facts.

The intended sequence is:

1. establish workforce skeleton;
2. inspect current work/process evidence;
3. infer missing operating-profile fields;
4. validate only what materially matters.

Do not deliver target-state process redesign before current work and authority are sufficiently understood.

## Targeted validation rules

### Auto-accept into baseline

May generally be accepted when:

- source is authoritative;
- record is current;
- no conflicting evidence exists;
- field is not especially consequential.

### Asynchronous confirmation

Use when:

- inference is high confidence;
- consequence is low/moderate;
- employee or manager can confirm cheaply.

### Consultant interview

Use when:

- evidence conflicts;
- field has high consequence;
- authority is unclear;
- workflow spans several functions;
- informal work is materially different from documents;
- interview itself is needed to understand incentives, risk, or exceptions.

### Workshop

Use when:

- several functions disagree on a shared process;
- no single person holds the whole workflow;
- target transformation requires shared understanding of the current state.

## Current-State Confidence Map

The primary discovery control artifact is the **Current-State Confidence Map**.

It should track, per material field:

- object ID;
- object type;
- field;
- current value;
- evidence state;
- confidence;
- evidence source(s);
- last verified date;
- validator / attestor if applicable;
- consequence if wrong;
- validation action;
- status.

This map determines where consultant time should be spent.

## Discovery exit criteria

Discovery does not require perfect knowledge.

A current-state baseline is sufficient when:

- active workforce is represented enough to route work;
- critical processes are understood enough to identify handoffs/owners;
- material systems and authoritative information classes are known;
- consequential current authority is documented or explicitly unresolved;
- material unknowns/disputes are visible;
- confidence is high enough to choose a transformation pilot safely;
- the organization can distinguish fact, observation, inference, and unknown.

## Transformation gate

After the baseline is adopted:

- begin target-state process/role/automation design;
- preserve discovery provenance;
- update the baseline when better evidence appears;
- do not treat the baseline as frozen forever.

## Consulting economics

The discovery system should reduce expensive human discovery by escalating uncertainty rather than treating every field equally.

Consultant time should be concentrated on:

- high-consequence ambiguity;
- cross-functional disagreement;
- undocumented authority;
- hidden process behavior;
- transformation-critical unknowns.

## Anti-patterns

Do not:

- interview everyone by default;
- ask clients to clean evidence before intake;
- infer authority from title;
- give one confidence score to an entire person/profile;
- mark AI inference as fact;
- redesign the target organization from an unvalidated org chart;
- build a detailed ontology before discovering what decisions it needs to support;
- spend workshop time confirming facts a system of record already proves.

## Required outputs

A completed discovery phase produces at least:

- discovery-mode declaration;
- evidence/source inventory;
- sponsor/authority record;
- current-state confidence map;
- working-plane/system inventory;
- current-process/pain-point summary;
- AI/automation readiness summary;
- unresolved unknowns/disputes;
- recommended high-value pilot;
- handoff/output package for client control-plane bootstrap and transformation.
