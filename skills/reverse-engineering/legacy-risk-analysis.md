# Legacy Risk Analysis Skill

## Purpose
Identify evidence-based modernization risks without prematurely prescribing a target architecture.

## Categories
- unsupported or aging runtime/frameworks
- tight coupling
- hidden business logic
- missing automated tests
- shared-database coupling
- stored-procedure dependency
- external-system dependency
- security limitations
- observability gaps
- deployment coupling
- maintainability risks

## Finding Format
- Finding
- Evidence
- Impact
- Confidence: HIGH / MEDIUM / LOW
- Possible Direction

## Output
Prefer `docs/reverse-engineering/09-risks.md`.

## Guardrails
Do not assign arbitrary numeric risk scores.
