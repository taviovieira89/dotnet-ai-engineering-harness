# Architecture Constraints Template

> **TEMPLATE:** Record only approved constraints. Use `PROPOSED` for unapproved choices and link material decisions to ADRs.

## Ownership and Boundaries

- **Capability / feature owner:** `[OWNER]`
- **Write ownership:** `[DATA_OR_RESOURCE_OWNER]`
- **Allowed dependencies:** `[CONTRACTS_AND_DIRECTION]`
- **Forbidden dependencies:** `[BOUNDARIES]`
- **Deployment boundaries:** `[CURRENT_AND_PROPOSED]`

## Contracts and Data

- **Public contracts:** `[API/EVENT/FILE_SCHEMA]`
- **Compatibility requirement:** `[POLICY]`
- **Data classification:** `[CLASSIFICATION]`
- **Source of truth and retention:** `[OWNER / POLICY]`
- **Sensitive data prohibited from logs/prompts:** `[CATEGORIES]`

## Security and Operations

- **Identity and authorization:** `[POLICY_REFERENCE]`
- **Tool permissions:** `[READ / WRITE / PRIVILEGED SCOPES]`
- **External dependencies:** `[APPROVED BOUNDARIES]`
- **Reliability and recovery:** `[RETRY / IDEMPOTENCY / RECOVERY]`
- **Observability requirements:** `[REDACTED SIGNALS AND CORRELATION]`
- **Required human approvals:** `[TRIGGERS / OWNER]`

## Status and Verification

- **Status:** PROPOSED / ACCEPTED / REJECTED / SUPERSEDED
- **Decision owner:** `[ROLE]`
- **ADR:** `[ADR_ID_OR_NONE]`
- **Enforcement:** `[TEST / POLICY / REVIEW / MANUAL]`
- **Verification evidence:** `[CHECKS]`
