# ADR-011 — Collect Privacy-Minimized AI Run Metadata

## Status

PROPOSED

## Context

Application monitoring alone may not show agent stages, tool retries, correction loops, review results, or human interventions. Full prompt logging creates unnecessary exposure.

## Decision

If AI observability is required, record governed run/stage metadata and outcomes while excluding prompt/completion content by default. Set retention, access, and deletion policy before collection.

## Rationale

Aggregate metadata supports quality and reliability analysis with lower data exposure.

## Consequences

- Positive: evidence for operating and improving the harness.
- Negative: telemetry cost, attribution uncertainty, and retention risk.

## Alternatives

No AI telemetry; full conversation capture; or minimized metadata. This example proposes the last option where a defined need exists.
