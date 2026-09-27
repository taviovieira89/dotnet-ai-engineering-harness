# DevOps Skill Category

**Classification: OPTIONAL by project; privileged operations require human approval.**

Use DevOps skills for build/release workflow, artifact integrity, environment configuration, deployment readiness, rollback, and infrastructure lifecycle.

## Recommended Scope

- Keep build and release evidence reproducible and tied to an immutable artifact.
- Separate environment configuration from source and protect secret values.
- Treat pipeline, infrastructure, deployment, and production access as `PRIVILEGED`.
- Require approvals, change evidence, health checks, and recovery plans for privileged changes.
- Never infer permission to mutate delivery systems from the existence of pipeline documentation.

## Skill Contract

Use [SKILL-TEMPLATE.md](../SKILL-TEMPLATE.md). Inputs include approved change plan, pipeline definitions, validation evidence, and rollback requirements. Outputs include release/operational plan and evidence. Read access is scoped; write/execute grants are provided by the harness. External access is explicitly allowlisted. Human approval is mandatory for deployment and infrastructure mutation.
