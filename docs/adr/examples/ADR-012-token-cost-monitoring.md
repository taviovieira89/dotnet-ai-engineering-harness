# ADR-012 — Monitor Token Usage and Estimated Cost

## Status

PROPOSED

## Context

Token volume and model pricing can affect execution cost and context capacity, but provider usage fields and cost allocation may be incomplete or change over time.

## Decision

Where provider data is available and policy permits, collect input/output/total token counts and estimate cost using a versioned rate source. Mark missing data and estimates explicitly; do not log content to derive usage.

## Rationale

Transparent, qualified measurements support budgeting without overstating accuracy.

## Consequences

- Positive: visibility into usage trends and approximate task attribution.
- Negative: pricing changes, shared-task attribution, and provider differences limit precision.

## Alternatives

No usage accounting; exact-cost claims from token counts alone; or versioned estimates with caveats. This example proposes the last option and no universal budget target.
