# ADR-003 — Establish Layered Agent Instructions

## Status

PROPOSED

## Context

Agents need consistent policies and task context, while a large or contradictory instruction set can reduce relevance and create unsafe ambiguity.

## Decision

Maintain a project-root `AGENT.md` for stable global rules and scope-specific guidance for local conventions. Define source precedence, owners, review cadence, and conflict escalation.

## Rationale

Layering supports both consistency and focused context selection.

## Consequences

- Positive: discoverable rules with fewer irrelevant instructions.
- Negative: overlaps and stale local rules need active governance.

## Alternatives

One monolithic instruction file; ad hoc prompts; or a small global file with owned local guidance. This example proposes the layered option.
