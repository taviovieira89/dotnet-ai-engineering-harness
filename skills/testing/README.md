# Testing Skill Category

**Classification: CORE validation practice; separate skill is OPTIONAL.**

Use testing skills to choose a risk-appropriate test level, create deterministic cases, diagnose failures, and report evidence accurately.

## Recommended Scope

- Trace cases to acceptance criteria and critical invariants.
- Select unit, integration, contract, architecture, end-to-end, performance, and security checks by risk.
- Prefer synthetic, deterministic test data; isolate external dependencies.
- Test negative paths, boundaries, retries, authorization, and recovery where relevant.
- Distinguish a failed test, an unrun test, and missing evidence.

## Skill Contract

Use [SKILL-TEMPLATE.md](../SKILL-TEMPLATE.md). Inputs include requirements, test strategy, source, fixtures, and validation results. Outputs include proposed/changed tests and reproducible result summaries. Read/write is limited to task-scoped test paths; execution permission is harness-controlled. No external access by default. Human approval is required before tests access production or restricted data.
