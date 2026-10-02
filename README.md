# Tenshodo Process

**A portable operating-system transformation playbook for building durable, AI-enabled organizations.**

Tenshodo Process is the consultancy methodology repository created from the operating-system work first developed inside Tenshodo Exchange.

It is designed to travel.

The repository contains the principles, engagement model, reusable playbooks, templates, maturity framework, and sanitized field evidence needed for a transformation team to enter a new organization and build a durable operating system without carrying the prior client's confidential data or blindly copying its org chart.

> New session? Start with [CONTINUE_HERE.md](CONTINUE_HERE.md).

## Consultancy premise

A modern organization should be able to answer, durably:

- What are we trying to accomplish?
- What work is active now?
- Who or what is authorized to execute it?
- What is the authoritative source for each important fact?
- What depends on what?
- What changed?
- What evidence proves completion?
- What happens next?
- Can a new employee, consultant, ChatGPT conversation, or agent resume safely without reconstructing history from meetings and memory?

Tenshodo Process helps clients build that capability.

## Engagement quick start

Once a client has been configured with a `PROCESS_CONTEXT.json`, the normal operator experience should be a one-line command:

> **Check Tenshodo-Process and execute Engagement Step 2 for <client>.**

Or, when the client is already unambiguous:

> **Check the process and execute Step 2.**

The resolver in [engagement/STEP_REGISTRY.json](engagement/STEP_REGISTRY.json) maps the step to the portable protocol in [docs/CONVERSATION_BOOTSTRAP_PROTOCOL.md](docs/CONVERSATION_BOOTSTRAP_PROTOCOL.md). It checks `PROCESS_CONTEXT.json` or `PROCESS_POINTER.json` first, follows any pointer to the client control plane, then reads live client state.

See [engagement/QUICK_START.md](engagement/QUICK_START.md).

The user should not need to paste the old launch prompt, role charter, task ID, or prior conversation history.

## What we carry between companies

We carry the methodology, patterns, schemas, playbooks, templates, evaluation criteria, engagement sequencing, and sanitized lessons learned.

We do **not** carry employee records, customer data, credentials, internal client financial data, proprietary product information, client operating state, private prompts containing client secrets, or anything else a consultant would not be entitled to take to a new engagement.

Every client receives its own control plane and working-plane architecture.

## Core model

The method separates five things that organizations often blur together:

1. **Working plane** — where people collaborate and create business artifacts.
2. **Durable control plane** — where state, authority, dependencies, decisions, and resumable work are maintained.
3. **Execution plane** — people, software, meetings, ChatGPT conversations, and agents that perform work.
4. **Adoption authority** — who can make a proposal binding.
5. **Evidence plane** — the sources that prove facts, completion, controls, and decisions.

GitHub has proven useful as the durable control plane, but the methodology is not tied to GitHub forever. The principle is durable, versioned, reviewable operational state.

## Role-conversation launch standard

A client role conversation should be launched from durable role metadata.

The long-form launch template remains available at [templates/ROLE_CONVERSATION_LAUNCH_PROMPT.md](templates/ROLE_CONVERSATION_LAUNCH_PROMPT.md), but normal engagements should prefer the step resolver + client context packet.

The launch instruction is an ignition key, not the source of truth. The live client control plane and declared authoritative systems override stale prompt text or prior conversation memory.

## Pattern maturity

Patterns in this repository are not automatically declared best practice.

They move through:

**Observed → Candidate Pattern → Validated → Portable**

Patterns that fail or are superseded become **Deprecated**.

The evidence matrix deliberately keeps newer management/AI patterns at candidate status until field experience supports more.

## Initial field laboratory

Tenshodo Exchange is the first field laboratory.

The flagship Phoenix XI project repeatedly demonstrated:

- zero-context resumption;
- bounded execution and checkpointing;
- machine-readable current-task state;
- live-source revalidation;
- working-plane/control-plane separation;
- deterministic recovery after interrupted sessions;
- no-dual-canonical rules.

The Tenshodo management transformation is now testing newer patterns:

- target accountability versus current execution authority;
- organizational bootstrap before the target org exists;
- AI role conversations that incubate functions;
- human stewardship transfer from durable AI-built state;
- employee suggestion → impact map → controlled adoption;
- company dependency graphs.

These newer patterns remain subject to validation.

## Repository map

- [PROCESS_STATE.json](PROCESS_STATE.json) — machine-readable methodology cursor
- [METHODOLOGY_ROADMAP.md](METHODOLOGY_ROADMAP.md) — methodology build plan
- [METHOD_RUNBOOK.md](METHOD_RUNBOOK.md) — how the methodology itself evolves and checkpoints
- [engagement/STEP_REGISTRY.json](engagement/STEP_REGISTRY.json) — stable engagement-step IDs and ordinals
- [engagement/QUICK_START.md](engagement/QUICK_START.md) — one-line conversation-start workflow
- [docs/CONVERSATION_BOOTSTRAP_PROTOCOL.md](docs/CONVERSATION_BOOTSTRAP_PROTOCOL.md) — context resolution algorithm
- [templates/PROCESS_CONTEXT.json](templates/PROCESS_CONTEXT.json) — client control-plane context packet template
- [templates/PROCESS_POINTER.json](templates/PROCESS_POINTER.json) — redirect template for specialized/non-control client repositories
- [decisions/DEC-0001-portable-method-and-client-boundary.md](decisions/DEC-0001-portable-method-and-client-boundary.md) — formal portable-method/client-state boundary
- [docs/CONSULTING_MODEL.md](docs/CONSULTING_MODEL.md) — how the team works as a consultancy
- [docs/METHOD_PRINCIPLES.md](docs/METHOD_PRINCIPLES.md) — portable principles
- [docs/ENGAGEMENT_LIFECYCLE.md](docs/ENGAGEMENT_LIFECYCLE.md) — client transformation sequence
- [docs/CLIENT_REPOSITORY_ARCHITECTURE.md](docs/CLIENT_REPOSITORY_ARCHITECTURE.md) — recommended client control-plane topology
- [docs/PORTABILITY_AND_CONFIDENTIALITY.md](docs/PORTABILITY_AND_CONFIDENTIALITY.md) — strict client boundary
- [docs/PATTERN_MATURITY_MODEL.md](docs/PATTERN_MATURITY_MODEL.md) — evidence-based promotion rules
- [patterns/PATTERN_REGISTRY.json](patterns/PATTERN_REGISTRY.json) — machine-readable pattern catalog
- [patterns/EVIDENCE_MATRIX.md](patterns/EVIDENCE_MATRIX.md) — maturity rationale and evidence gaps
- [playbooks/](playbooks/) — reusable execution guides
- [templates/](templates/) — client-safe starter artifacts
- [case-studies/](case-studies/) — sanitized field evidence
- [worklogs/](worklogs/) — development history of the methodology

## Public-repository rule

This repository is public.

Only portable, sanitized, consultancy-safe material belongs here.

Client-specific state belongs in the client's own authorized repository or systems.

## Scope

Tenshodo Process is methodology.

Tenshodo Exchange Management is one company's management control plane.

Tenshodo Exchange is one specialized project control plane.

Never collapse those scopes.
