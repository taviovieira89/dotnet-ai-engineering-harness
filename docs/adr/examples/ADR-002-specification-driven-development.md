# ADR-002 — Adopt Specification-Driven Development

## Status

PROPOSED

## Context

Teams need traceability from intent to implementation and validation, but full specification overhead may not suit every task.

## Decision

For non-trivial changes, use a concise specification, testable acceptance criteria, architecture constraints, and an approved implementation plan. Use a lightweight record for low-risk work.

## Rationale

Explicit expected outcomes reduce ambiguity and support independent review.

## Consequences

- Positive: improved traceability and earlier discovery of missing decisions.
- Negative: specifications require maintenance and accountable owners.

## Alternatives

Ticket-only implementation; heavyweight specification for all changes; or risk-proportional SDD. This example proposes risk-proportional SDD.
