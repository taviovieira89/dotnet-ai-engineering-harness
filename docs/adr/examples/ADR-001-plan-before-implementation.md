# ADR-001 — Plan Before Non-Trivial Implementation

## Status

PROPOSED

## Context

Unplanned changes can miss ownership boundaries, acceptance criteria, security impact, and verification. Planning itself has a cost, especially for trivial tasks.

## Decision

Require risk-proportional scope and verification planning before non-trivial AI implementation. Permit a concise analysis for small, low-risk changes.

## Rationale

This surfaces unknowns early without imposing a heavyweight process on every edit.

## Consequences

- Positive: clearer scope, risks, and validation evidence.
- Negative: planning can become ceremony unless kept proportional.

## Alternatives

Start coding immediately for all work; require full plans for all changes; or scale planning to risk. This example proposes the risk-proportional option.
