# Test Review Skill

## Purpose
Assess whether automated tests provide proportionate evidence for the behavior and regression risk of a change.

## Checks
- Trace tests to acceptance criteria and critical behavior.
- Evaluate appropriate mix of unit, integration, architecture, API, database, frontend, and end-to-end tests.
- Check important success, failure, boundary, authorization, and regression paths where applicable.
- Prefer behavior assertions over fragile implementation-detail assertions.
- Identify missing characterization tests when legacy behavior is being changed.
- Never claim tests passed unless execution evidence is available.

## Output
Report missing material coverage separately from optional test improvements.
