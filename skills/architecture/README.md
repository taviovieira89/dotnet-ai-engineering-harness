# Architecture Skill Category

**Classification: CORE architectural guidance; separate skill is OPTIONAL.**

Use architecture skills to identify capability ownership, dependency direction, quality attributes, contracts, evolution drivers, and ADR needs.

## Recommended Scope

- Analyze the smallest relevant boundary before proposing changes.
- Separate current implementation evidence from target state and recommendations.
- Prefer explicit contracts and stable ownership over cross-boundary internals.
- Evaluate operational cost and measured drivers before introducing distributed systems or broad abstractions.
- Escalate conflicting requirements or decisions outside delegated authority.

## Skill Contract

Use [SKILL-TEMPLATE.md](../SKILL-TEMPLATE.md). Inputs include scope, approved architecture, ADRs, quality attributes, and relevant design evidence. Outputs include boundary analysis, options, risks, and an ADR when requested. Read permission is relevant docs/source only; write permission is none by default for review skills. No external access by default. Human approval is required for material architecture decisions.
