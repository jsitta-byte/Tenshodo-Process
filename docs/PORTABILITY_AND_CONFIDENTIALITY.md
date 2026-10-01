# Portability and Confidentiality

## Rule

The methodology travels.

Client data does not.

## Public repository status

Tenshodo Process is a public repository.

Never commit:

- employee personal information;
- client financial details;
- customer lists;
- credentials or secrets;
- contracts;
- confidential security architecture;
- proprietary pricing;
- private internal communications;
- client-specific prompt context that exposes confidential information;
- raw client documents.

## Safe field evidence

Case evidence should be abstracted.

Good:

> A long-running research project repeatedly hit conversation limits. A durable state file, deterministic source ledger, and batch checkpoint protocol allowed new sessions to resume without redoing completed work.

Bad:

> Copying a private client's exact employee records, sales data, or security configuration to prove the pattern worked.

## Client-owned state

Each client's operating state stays in:

- client-authorized repositories;
- client SharePoint/Drive;
- client business systems;
- explicitly approved engagement storage.

## Consultancy intellectual property

Reusable abstractions may be captured in this repository when they are:

- sanitized;
- not contractually restricted;
- not dependent on confidential client facts;
- expressed at the pattern/playbook/template level.

## Clean-room test

Before bringing a lesson into Tenshodo Process, ask:

> Could a consultant explain and use this pattern at a new company without knowing which prior client produced it?

If no, abstract further or leave it in the client environment.

## Exit from an employer or client

Do not interpret "portable methodology" as permission to take materials you do not own or have the right to retain.

Carry the public method.

Leave protected business information behind.
