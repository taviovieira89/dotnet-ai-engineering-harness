# Frontend Skill Category

**Classification: OPTIONAL by project.**

Use frontend skills for UI architecture, accessibility, state and data flow, client-side validation, API adaptation, performance, and component testing.

## Recommended Scope

- Keep user-interface behavior within clear feature boundaries.
- Treat client-side permissions as presentation only; authoritative access checks belong at the trusted service boundary.
- Include loading, empty, error, retry, conflict, and access-denied behavior where relevant.
- Follow the selected project's approved framework, design system, accessibility standard, and localization policy.
- Keep secrets and privileged operations out of client code.

## Skill Contract

Use [SKILL-TEMPLATE.md](../SKILL-TEMPLATE.md). Inputs should include the feature spec, API contract, relevant UI code, and accessibility constraints. Outputs should include scoped implementation guidance and component/interaction validation. Read only relevant frontend paths; write permission comes from the harness. External access is none by default. Human approval is required for framework/design-system changes where project policy says so.
