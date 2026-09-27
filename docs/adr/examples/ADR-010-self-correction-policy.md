# ADR-010 — Bound Autonomous Correction Attempts

## Status

PROPOSED

## Context

Automated implementation/review loops can converge on defects, repeat changes, or consume unbounded resources.

## Decision

Set a configurable `MAX_AGENT_CORRECTION_ATTEMPTS`. Require re-validation and independent review after every correction. Stop and require `HUMAN_REVIEW_REQUIRED` when the limit is reached, progress fails to converge, or new ambiguity appears.

## Rationale

Bounded attempts preserve useful self-correction without granting unlimited autonomy.

## Consequences

- Positive: limits cost, repeated unsafe changes, and runaway execution.
- Negative: an overly small limit may escalate routine work; calibrate per project.

## Alternatives

No automated correction; unbounded correction; or bounded correction with escalation. This example proposes the bounded option and sets no universal numeric value.
