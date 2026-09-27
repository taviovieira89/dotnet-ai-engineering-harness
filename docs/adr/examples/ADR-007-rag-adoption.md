# ADR-007 — Use RAG for Governed Knowledge Retrieval

## Status

PROPOSED

## Context

Large or frequently updated documentation may not fit a useful static context. Retrieval can also expose stale, unauthorized, or instruction-injected content.

## Decision

Adopt RAG only for a defined retrieval need with source ownership, ACL-aware search, provenance, freshness, deletion, and evaluation. Keep authoritative instructions outside the knowledge index.

## Rationale

Retrieval can improve relevance when curated static context or direct search is insufficient.

## Consequences

- Positive: on-demand access to larger approved knowledge sets.
- Negative: ingestion, indexing, access-control, freshness, and poisoning risks.

## Alternatives

Static context; direct search; unrestricted retrieval; or governed RAG. This example proposes the last option only when justified.
