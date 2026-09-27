# ADR-009 — Require Human Approval for Reserved Decisions

## Status

PROPOSED

## Context

Business risk, security exceptions, production changes, and ambiguous requirements require accountability that an agent may not possess.

## Decision

Require a named human decision for configured high-impact, privileged, irreversible, security-sensitive, or ambiguous actions. Record scope, evidence, result, and approver.

## Rationale

Human authority remains explicit while agents can safely prepare options and evidence.

## Consequences

- Positive: accountable risk acceptance and controlled external effects.
- Negative: requires available owners and clear approval turnaround.

## Alternatives

Agent inference; human approval for every action; or risk-based human approval. This example proposes the risk-based pattern.
