# Integration Skill Category

**Classification: OPTIONAL by project.**

Use integration skills for provider contracts, adapters, authentication boundaries, rate limits, error mapping, retries, idempotency, reconciliation, and contract testing.

## Recommended Scope

- Keep provider-specific protocols behind an adapter or anti-corruption boundary.
- Use approved schemas and synthetic fixtures; label uncertain fields and semantics.
- Define timeouts, retryability, idempotency, partial results, rate limits, and recovery.
- Do not expose provider credentials or internal protocol identifiers to unrelated layers.
- Require human approval for external writes, permission expansion, and production changes.

## Skill Contract

Use [SKILL-TEMPLATE.md](../SKILL-TEMPLATE.md). Inputs include canonical contracts, provider requirements, data classification, and failure semantics. Outputs include adapter design, mapping, tests, and operational notes. Read/write scopes are task-specific; external-system access is denied by default and separately granted. Human approval is required for live writes and privileged access.
