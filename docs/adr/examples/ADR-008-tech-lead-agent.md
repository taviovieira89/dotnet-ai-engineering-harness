# ADR-008 — Use an Independent Tech Lead Agent

## Status

PROPOSED

## Context

Implementation authors should not be the only source of assurance for architecture, requirements, tests, and security.

## Decision

Use a read-only reviewer independent of implementation for changes required by project risk policy. Keep final authority with accountable humans for reserved decisions.

## Rationale

Independent review makes findings and evidence explicit while avoiding self-approval.

## Consequences

- Positive: repeatable review and separation of duties.
- Negative: quality depends on context, reviewer calibration, and maintenance of review policy.

## Alternatives

Self-review only; unrestricted reviewer; or independent read-only review. This example proposes the read-only pattern.
