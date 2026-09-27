# Observability Skill Category

**Classification: CORE to define required evidence; AI-specific collection is OPTIONAL.**

Use observability skills to define useful, privacy-conscious application and AI execution signals, traces, dashboards, alerts, and evaluation evidence.

## Recommended Scope

- Separate application telemetry from model/harness telemetry.
- Correlate run and stage metadata without retaining full prompts or sensitive tool arguments by default.
- Define metric formulas, denominators, missing-data behavior, ownership, retention, and project-specific targets.
- Track validation/review outcomes and human interventions without rewarding unsafe autonomy.
- Review access to telemetry as access to potentially sensitive project metadata.

## Skill Contract

Use [SKILL-TEMPLATE.md](../SKILL-TEMPLATE.md). Inputs include telemetry policy, event schemas, run metadata, and evaluation questions. Outputs include metric definitions, instrumented events, dashboard/alert proposals, and validation evidence. Read/write permissions are scoped to observability code/config/docs; access to telemetry stores is separately authorized. No prompt-content access by default. Human approval is required for sensitive-data collection or retention changes.
