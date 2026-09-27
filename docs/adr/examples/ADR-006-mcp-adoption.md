# ADR-006 — Adopt MCP for Shared Tool Interfaces

## Status

PROPOSED

## Context

Multiple agent clients may benefit from a standardized tool interface, but a protocol server also adds operational and security responsibilities.

## Decision

Adopt MCP only where shared discovery, resource, or tool semantics justify operating a server. Retain harness and server-side authorization; MCP does not imply access approval.

## Rationale

This balances interoperability with least privilege and operational simplicity.

## Consequences

- Positive: consistent tool interface across supported clients.
- Negative: additional server, authentication, authorization, monitoring, and incident surface.

## Alternatives

Direct integration for every client; unrestricted protocol server; or narrowly scoped MCP where reuse justifies it. This example proposes evaluating the last option.
