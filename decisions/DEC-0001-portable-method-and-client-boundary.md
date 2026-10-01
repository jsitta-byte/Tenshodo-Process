# DEC-0001 — Portable Method and Client Boundary

- **Status:** Adopted
- **Date:** 2026-10-01
- **Decision class:** Consultancy architecture
- **Applies to:** Tenshodo Process
- **Adoption authority:** Tenshodo Process founding sponsor

## Context

The Tenshodo management team intends to carry this operating-system transformation work from organization to organization as a consultancy.

A portable method creates value only if it can travel without creating confidentiality, ownership, or source-of-truth problems.

## Decision

### 1. Tenshodo Process contains methodology, not client state

This repository may contain:

- principles;
- playbooks;
- templates;
- schemas;
- maturity criteria;
- sanitized case evidence;
- reusable consulting operating practices.

It must not contain live client operational state or confidential source material.

### 2. Each client receives a separate authorized operating environment

Client transformation state belongs in client-specific repositories and systems with appropriate access.

### 3. Portability must not rely on proprietary client facts

A pattern should be understandable and usable without access to the client that originated it.

### 4. Public-repository standard

Because Tenshodo Process is public, every contribution must pass a confidentiality and ownership check before commit.

### 5. Method evolution is evidence-based

Tenshodo remains the first field laboratory, not the universal template.

Patterns gain maturity through evidence and may be changed or deprecated.

## Consequences

- No raw employee/customer/client data in Tenshodo Process.
- Case studies are sanitized.
- Client repository templates remain generic.
- Engagement teams maintain a logical firewall between methodology and client operating state.
- Consultants leaving a client carry the method only to the extent they have the right to do so.

## Revisit triggers

- Repository visibility changes.
- Consulting contracts change IP/retention rights.
- The team begins supporting regulated or specially restricted environments.
- A pattern cannot be generalized without confidential implementation details.
