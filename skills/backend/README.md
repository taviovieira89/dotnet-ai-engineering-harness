# Backend Skill Category

**Classification: OPTIONAL by project.**

Use backend skills for API boundaries, application use cases, domain invariants, persistence ownership, integration adapters, error semantics, resilience, and service testing.

## Recommended Scope

- Keep domain and policy independent of transport, persistence, and provider SDKs.
- Make ownership and transactions explicit; avoid cross-owner writes.
- Validate inputs at boundaries and protect invariants in the owning domain/application layer.
- Use standardized, non-sensitive error responses.
- Design retries, idempotency, concurrency, and asynchronous work according to actual requirements.

## Skill Contract

Use [SKILL-TEMPLATE.md](../SKILL-TEMPLATE.md). Inputs should include the approved specification, API schema, relevant module, data constraints, and tests. Outputs should include a vertical-slice implementation approach and relevant validation. Read/write access is limited to task-scoped backend paths through the harness. External access is none by default; human approval is required for new platforms, data-boundary changes, or security exceptions.
