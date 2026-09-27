# Security Skill Category

**Classification: CORE security policy; separate skill is OPTIONAL.**

Use security skills for threat analysis, secure design, data classification, authorization, secret handling, dependency risk, and security validation.

## Recommended Scope

- Identify trust boundaries, assets, actors, abuse cases, and residual risk.
- Enforce least privilege outside the model and reauthorize tool calls at execution.
- Treat user, retrieved, model, and tool output as untrusted.
- Minimize sensitive context and keep secrets out of prompts, source, and telemetry.
- Escalate security exceptions and material uncertainty to an accountable human.

## Skill Contract

Use [SKILL-TEMPLATE.md](../SKILL-TEMPLATE.md). Inputs include architecture, data classifications, threat model, and change evidence. Outputs include findings, mitigations, required checks, and escalation decisions. Read access is limited to authorized security materials; no secret access by default. Write access is limited to approved security docs/tests. Privileged actions require security-owner approval.
