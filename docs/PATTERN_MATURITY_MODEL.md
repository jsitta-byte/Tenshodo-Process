# Pattern Maturity Model

Tenshodo Process distinguishes useful observations from portable doctrine.

## States

### Observed

A meaningful behavior, problem, or solution has been seen in the field.

Evidence may be narrow or anecdotal.

### Candidate Pattern

The team believes the observation may generalize.

The pattern has:

- a named problem;
- proposed mechanism;
- expected outcome;
- known assumptions.

It has not yet earned strong confidence.

### Validated

The pattern has worked repeatedly in meaningful use.

Validation should include:

- repeated execution;
- recovery from failure/interruption where relevant;
- evidence of the intended outcome;
- known operating conditions.

Validation inside one organization is valuable but does not automatically prove portability.

### Portable

The pattern has demonstrated usefulness across materially different environments or has equivalent strong evidence that its abstraction survives differences in:

- organization;
- domain;
- tools;
- authority;
- workforce;
- scale.

Portable patterns should identify implementation choices separately from core principles.

### Deprecated

Evidence shows the pattern is harmful, obsolete, misleading, or superseded.

Deprecation should preserve the reason so the team does not rediscover the same failure.

## Promotion questions

Before promotion, ask:

1. What problem does this solve?
2. What evidence says it solved it?
3. Under what conditions?
4. What failed?
5. What is tool-specific versus conceptual?
6. What would falsify the pattern?
7. Has a materially different environment tested it?
8. What would a new consultant need to implement it safely?

## Evidence standard

Pattern status changes should be checkpointed in the pattern registry and supported by sanitized field notes.

Do not promote by enthusiasm.
