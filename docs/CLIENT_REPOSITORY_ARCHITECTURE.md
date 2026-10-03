# Client Repository Architecture

## Purpose

Each client engagement requires its own authorized durable control plane.

Do not use the public Tenshodo Process repository as the client's operating repository.

## Recommended minimum

A new client control-plane repository should begin small:

```
README.md
CONTINUE_HERE.md
COMPANY_STATE.json
TRANSFORMATION_PLAN.md
OPERATING_RUNBOOK.md
CHANGELOG.md
decisions/
worklogs/
docs/
registries/
roles/
templates/
```

Not every directory must be populated immediately.

## Minimum durable objects

### CONTINUE_HERE

Answers:

- what to read;
- what not to assume;
- how to verify live state;
- where the current cursor is.

### State file

Machine-readable current truth such as:

- phase;
- task;
- dependencies;
- current executor;
- target owner;
- exact next action;
- external source refs;
- invariants.

### Human plan

Explains the larger program and definitions of done.

### Runbook

Explains startup, execution, validation, checkpoint, recovery, and session-end behavior.

### Decisions

Preserve decisions that should survive employee or consultant turnover.

### Worklog

Append-oriented execution evidence.

## Client-specific authority

The client repository should point to client systems rather than copying every business artifact into Git.

Examples:

- ERP remains authoritative for transactions;
- HRIS remains authoritative for employment records;
- CRM remains authoritative for customer/opportunity state;
- SharePoint may remain authoritative for controlled business documents;
- Git may be authoritative for transformation state and operating architecture.

## Specialized repositories

A client may need specialized project/data/software repositories.

The management/control-plane repository should summarize and link rather than absorb every execution detail.

## Exit standard

Before the consulting team exits, a zero-context qualified client operator should be able to resume from the repository without access to private consultant chat history.

## Working-plane topology

Working plane is a functional concept, not a requirement that one organization use one collaboration system.

A client may have multiple approved working-plane instances across providers, tenants, environments, services, and locations.

Model material environments with stable IDs and keep their identity distinct:

**provider → tenant/account → environment → service → location**

The control plane should record pointers, authority assignments, and material flows rather than duplicate every working artifact.

Use:

- templates/ENVIRONMENT_REGISTRY.json;
- templates/INFORMATION_AUTHORITY_REGISTER.json;
- templates/INFORMATION_FLOW_REGISTRY.json.

The rule remains one declared authority per information class, not one cloud per organization.
