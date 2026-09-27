# ADR-004 — Separate Skills from Permissions

## Status

PROPOSED

## Context

Reusable technical knowledge helps agents act consistently, but instructional content is not an enforceable access-control mechanism.

## Decision

Define skills with a common contract for purpose, scope, inputs, outputs, tools, context, permissions, restrictions, validation, and approval. Enforce tool permissions independently in the harness.

## Rationale

Separating guidance from capabilities prevents accidental permission expansion.

## Consequences

- Positive: portable skills and auditable tool boundaries.
- Negative: more explicit metadata to maintain.

## Alternatives

Prompt-only conventions; broad agents with implicit tools; or declarative skills and external permission enforcement. This example proposes the latter.
