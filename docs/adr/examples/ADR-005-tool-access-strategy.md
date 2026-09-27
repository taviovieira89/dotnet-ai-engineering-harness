# ADR-005 — Govern Tool Access by Capability

## Status

PROPOSED

## Context

Agents may need repository, validation, or external-system tools. Unrestricted tool access increases risk and makes audit difficult.

## Decision

Grant task-scoped, least-privilege read/write capabilities. Deny privileged operations by default and require configurable human approval, audit, and recovery controls.

## Rationale

The tool boundary should enforce the same risk policy as human-operated automation.

## Consequences

- Positive: smaller blast radius and attributable actions.
- Negative: capability policy and approval flow require maintenance.

## Alternatives

Unrestricted access; read-only-only access; or task-scoped tiers with human approval for privilege. This example proposes the tiered model.
