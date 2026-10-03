# Working-Plane Topology

## Purpose

Provide a provider-neutral 10XP model for organizations whose human/operational work spans one or many clouds, tenants, environments, services, and locations.

## Core rule

**One organization may have many working-plane instances. Each material information class still has one declared authority at a time.**

Do not confuse provider, tenant/account, environment, service, location, and information authority. These are separate dimensions.

## Environment identity

Use this hierarchy when applicable:

**provider → tenant/account → environment → service → location**

A provider name alone is not sufficient evidence provenance when multiple environments may exist.

## Environment Registry

Every material environment should receive a stable ID and describe provider, tenant/account/domain, environment classification, services, business purpose, owner/steward, allowed information classes, access boundary, and lifecycle state.

See templates/ENVIRONMENT_REGISTRY.json.

## Authority

Assign authority separately from storage location.

Use the Information Authority Register to answer which information class is authoritative where and whether another location is a working copy, replica, export, archive, or superseded copy.

The method does not require one provider to own all organizational truth.

## Information flows

Material cross-environment movement should be modeled as a governed flow with source, destination, direction, information class, transformation, authority behavior, validation, failure/staleness behavior, and owner.

See templates/INFORMATION_FLOW_REGISTRY.json.

## Complexity levels

### Level 1 — simple topology

Use for small organizations with a few clearly separated systems.

### Level 2 — multi-system / multi-tenant

Add environment IDs, authority assignments, material locations, and major flows.

### Level 3 — complex enterprise / regulated

Add jurisdiction, classification, identity boundaries, retention, integration dependencies, deployment environments, and stronger access controls.

**Model complexity where it exists; do not manufacture it where it does not.**

## AI / connector rule

A connected AI session must not infer that a search result is relevant merely because the filename or contents match.

The result must belong to an authorized in-scope environment or be explicitly recorded as out-of-scope evidence.

## Relationship to durable control

The working-plane topology describes where organizational work and authoritative business information live.

The durable control plane describes state, authority, dependencies, decisions, resumability, and pointers needed to govern that work.

Do not duplicate every working artifact into the control plane merely to make the control plane central.
