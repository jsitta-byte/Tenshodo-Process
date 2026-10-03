# Parallel Workstream Model

## Purpose

A mature engagement may need several governed functions to execute at the same time.

A single global `current_task_id` is useful during early bootstrap, but it should not force sequential execution once distinct functions have real durable work.

This model allows one engagement control plane to coordinate multiple **parallel workstreams** without collapsing role boundaries or creating separate client control planes.

## Core rule

**One engagement may contain many workstreams. Each workstream has one declared current executor and one durable current-task cursor at a time.**

Workstreams are coordination lanes, not new organizations.

Examples:

- operating model / governance;
- commercialization / brand;
- revenue / sales;
- product / service design;
- technology;
- data / AI;
- people;
- finance;
- legal / risk;
- security.

Do not create a workstream merely to mirror an org chart. Create one when real durable work can proceed independently enough to justify its own executor, cursor, and checkpoint history.

## Workstream object

Each active workstream should record at least:

- stable `workstream_id`;
- name;
- purpose / outcome;
- lifecycle state;
- current task;
- current executor;
- target accountable role, when known;
- authority / adoption boundary;
- dependencies;
- next action;
- latest checkpoint;
- working-plane pointers;
- relevant authoritative sources;
- whether human action is currently required.

Use `templates/WORKSTREAM_REGISTRY.json` as the portable starter shape.

## Stable IDs

Prefer short durable IDs that describe the capability rather than a temporary person.

Examples:

- `OPS` — operating model / governance;
- `COM` — commercialization / brand;
- `REV` — revenue / sales;
- `PROD` — product / service portfolio;
- `TECH` — technology;
- `DATA` — data / AI;
- `PEOPLE` — people / organization;
- `FIN` — finance;
- `RISK` — legal / risk;
- `SEC` — security.

Clients may use different IDs when local terminology is better.

## Relationship to roles

A role conversation and a workstream are different objects.

A role conversation is an execution identity and governed perspective.

A workstream is a durable lane of work.

One role conversation may support more than one workstream only when its charter explicitly permits it and the role remains the declared executor for each workstream.

One workstream may change executors over time through a durable handoff.

Do not use a workstream to bypass the role-routing guard.

## Relationship to engagement steps

Engagement steps remain shared across the engagement.

Most parallel execution occurs inside `ENG-03 — Execute bounded client work and checkpoint`.

`ENG-04` may be invoked for a decision/adoption event in one workstream while other workstreams continue eligible `ENG-03` work.

`ENG-05` may transfer stewardship for one workstream without forcing unrelated workstreams to stop.

`ENG-06` closes or transitions the engagement only when engagement-level exit criteria are satisfied.

## Workstream routing

Before substantive work, resolve the client control plane and the conversation role-binding state first.

Then resolve the workstream:

1. If the user explicitly names a workstream, validate it against live durable state.
2. If the conversation is role-bound and exactly one active workstream is assigned to that role, route there automatically.
3. If the client declares a valid default workstream for that role/conversation, use it.
4. If exactly one active workstream exists for the engagement, route there automatically.
5. If several eligible workstreams remain, ask only which workstream the human wants to continue.

Never guess a workstream based only on prior conversational subject matter when live durable routing exists.

## Human command patterns

Single-workstream or unambiguous engagement:

> Check Tenshodo-Process and execute the current engagement step for <client>.

Multi-workstream engagement:

> Check Tenshodo-Process and continue the <workstream> workstream for <client>.

Examples:

> Check Tenshodo-Process and continue the commercialization workstream for Example Company.

> Check Tenshodo-Process and continue workstream COM for Example Company.

The human should not need to know the current task or role ID.

## Role firewall across workstreams

Parallelism must not weaken context boundaries.

- A CHRO-bound chat does not become CTIO because `TECH` is active.
- A CMO-bound chat does not perform CRO work unless durable state explicitly delegates that work and the charter permits it.
- Role-local assumptions do not become cross-functional truth.
- Shared facts cross workstreams through durable client state or another declared authoritative source.

## Dependencies

Workstreams may depend on one another without becoming sequential by default.

Record dependencies as:

- hard blocker — downstream work cannot safely proceed;
- soft dependency — work may proceed with assumptions marked;
- consultation — another role/workstream should review;
- adoption dependency — work can be built but not adopted until another decision occurs.

Example:

A commercialization workstream may draft positioning while a product workstream refines the service package, but final externally approved claims may have a hard dependency on validated offer scope.

## Checkpoint contract

Each bounded workstream batch should record:

- workstream ID;
- completed task/batch;
- current executor after checkpoint;
- evidence;
- unresolved assumptions;
- cross-workstream dependencies created or closed;
- exact next action;
- Next-Step Contract outcome.

## Portfolio / engagement roll-up

The engagement control plane should be able to answer:

- which workstreams are active;
- which are blocked;
- which require human action;
- which role conversation owns each;
- what cross-workstream dependencies are material;
- what has changed since the last operating review.

Do not force all workstream details into `PROCESS_CONTEXT.json`. Keep that packet pointer-oriented and reference the live workstream registry.

## Migration from a single cursor

A client does not need parallel workstreams on day one.

Start with the simpler single-cursor model.

Introduce the workstream registry when at least two durable bodies of work can proceed with distinct executors or independent checkpoints.

Until then, avoid extra structure.

## Definition of success

Parallel workstreams are successful when several functions can make progress concurrently while:

- each task has one declared current executor;
- role conversations remain role-bound;
- shared facts remain evidence-backed;
- cross-workstream dependencies are visible;
- human operators can still resume work from a short Process command;
- no workstream silently becomes a second client control plane.
