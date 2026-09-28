# Security Review Skill

## Purpose
Perform a focused engineering security review within the Tech Lead Agent's read-only authority.

## Checks
- Authentication and authorization boundaries.
- Input validation and output handling.
- Secret/configuration exposure.
- Sensitive data in logs or errors.
- API and browser protections where applicable.
- Dependency/configuration changes that alter security posture.
- Auditability requirements.
- High-impact security decisions requiring human approval.

## Rules
Do not expose secret values in findings. Report the location/category and remediation outcome instead. Escalate material uncertainty or risk acceptance to HUMAN_REVIEW_REQUIRED.
