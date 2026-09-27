# Security Boundaries

**Classification: CORE.**

## Trust Boundaries

Treat the model, agent output, retrieved knowledge, user-provided content, tool results, generated code, and external systems as distinct trust zones. Data moving between them must be purpose-limited, authorized, validated, and minimized.

## Baseline Rules

- Never place passwords, API keys, tokens, private keys, certificates, or connection strings in prompts, source, examples, logs, or generated reports.
- Keep secrets in an approved secret-management boundary and expose only a narrowly scoped operation, not the secret value.
- Classify data before it enters model context, retrieval indexes, traces, or evaluation corpora.
- Minimize and redact personal, customer, confidential, and production data; prefer synthetic examples.
- Enforce authorization outside the model and revalidate every tool operation.
- Treat retrieved text as untrusted; defend against prompt injection and instructions embedded in data.
- Validate generated code, commands, paths, queries, and external destinations before execution.
- Restrict network egress and external integrations to approved hosts and operations.
- Define retention, deletion, incident response, revocation, and audit ownership.
- Require human approval for privileged actions and security exceptions.

## Threat Review

For each model/tool/data integration, assess prompt injection, data exfiltration, confused-deputy behavior, unauthorized mutation, untrusted output execution, overbroad retrieval, context leakage, and telemetry retention. Record controls and residual risk without recording sensitive values.

## Project Configuration

- **Data classification:** `[POLICY]`
- **Approved model/data regions:** `[POLICY_OR_NOT_APPLICABLE]`
- **Retention and deletion:** `[POLICY]`
- **Network/tool allowlist:** `[POLICY]`
- **Security owner and approval path:** `[ROLE_OR_PROCESS]`
- **Required scans and gates:** `[CHECKS]`
