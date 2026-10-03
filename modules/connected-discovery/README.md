# Connected Discovery Module

## Purpose

Optional 10XP module for accelerating current-state discovery through authorized AI access to client systems when that access is appropriate.

Connected Discovery is not mandatory. A client with mature process documentation may use corpus intake only.

## Acquisition profiles

### Corpus only

Use client-provided process databases, SOP libraries, Human Operating Guides, system inventories, architecture records, and other current sources. No live connectors are required.

### Corpus + targeted connected validation

Use the corpus as the primary model, then connect only selected systems/environments to validate high-value gaps, drift, or contradictions.

### Targeted connected read

Use approved read-only access to named environments/locations where current evidence is otherwise insufficient.

### Broad connected read

Use only where low documentation maturity makes broader authorized evidence review economically justified.

### Controlled action mode

Not a discovery default. Any write/action capability is separately authorized and governed as transformation/operations work.

## Default posture

**Read source systems; write discovery outputs only to the approved discovery workspace/control environment.**

Discovery access does not grant adoption authority or permission to modify source systems.

## Scope contract

Before connected discovery, identify sponsor/authorization; enumerate environment IDs; identify provider/tenant/environment/service/location; declare allowed and prohibited data classes; record read/write capability separately; record retention/export restrictions; record access expiry/revocation; and establish out-of-scope-result handling.

Use templates/CONNECTED_DISCOVERY_SCOPE.json.

## Discovery behavior

Connected Discovery may inventory systems/locations; observe workflow evidence; reconstruct candidate process steps and handoffs; identify candidate authoritative information classes; identify recurring artifacts; identify candidate Benchmarks/checkpoints; detect contradictions; draft current-state process descriptions and SOPs; and propose validation questions.

It must not infer consequential authority from system usage, treat observed behavior as adopted policy, treat a wrong-tenant artifact as evidence, write to operational systems unless separately authorized, make generated SOPs binding, or carry confidential client state into the public 10XP repository.

## Process Evidence Graph

When useful, create a provisional graph connecting processes, roles, systems/environments, information classes, artifacts, approvals, controls, handoffs, exceptions, Benchmarks/checkpoints, and evidence sources.

Use templates/PROCESS_EVIDENCE_GRAPH.json or a client-native equivalent.

## SOP drafting

AI-generated SOPs are discovery outputs. They should identify evidence/provenance, confidence/unknowns, systems/environments, inputs/outputs, approvals/controls, exceptions, candidate Benchmarks, and validation needs.

Their maximum state is normally draft/proposed until appropriate human validation/adoption.

## Mature clients

Do not make mature clients rediscover what they already know.

If a trustworthy process corpus exists, ingest it first and use connected discovery selectively to test currentness, exceptions, and drift.

## Success

The module succeeds when it reduces low-value interview burden while preserving tenant/environment identity, authority boundaries, evidence state, provenance, confidentiality, targeted human validation, and human adoption.
