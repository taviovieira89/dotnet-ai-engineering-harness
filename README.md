# AI Engineering Architecture Starter Kit

## Purpose

This kit provides a project-independent operating model for AI-assisted software delivery. It combines clear requirements, risk-proportional planning, controlled tool access, automated validation, independent review, human escalation, and measurable feedback.

It is a **TEMPLATE**, not a ready-made policy. A adopting project must review the scope, data classification, technology guidelines, access boundaries, approval owners, and quality gates before using it. Generic **EXAMPLE** material demonstrates adaptation only and is not an approved business rule.

## Start Here

1. Copy and tailor [AGENT.md](AGENT.md) at the project root.
2. Define project security policy, architecture rules, and owners before granting agents tools.
3. Use the [SDD templates](docs/sdd/README.md) for non-trivial work.
4. Select only the agent roles, skills, MCP integrations, and retrieval capabilities the project needs.
5. Define validation commands, human approval points, and a project-specific Definition of Done.

## Core and Optional

| Classification | Practices |
| --- | --- |
| **CORE** | Agent instructions; security-first context; clear requirements and acceptance criteria; planning before non-trivial implementation; architecture constraints; least privilege; automated validation; human escalation; risk-appropriate review; auditable Definition of Done. |
| **OPTIONAL** | Separate specialist agents; multi-agent orchestration; MCP; RAG; external work-management or delivery integrations; dedicated observability agent; token/cost dashboards; bounded autonomous correction. |

An optional capability should have an owner, use case, threat review, permission model, failure behavior, and an ADR when it changes architecture or risk. More automation is not automatically better.

## Agent Baseline

- **Implementation Agent: REQUIRED** when an agent is authorized to change project files.
- **Planning Agent: RECOMMENDED** as a separate role; planning itself is CORE for non-trivial work and may be combined with implementation for small tasks.
- **Tech Lead Agent: RECOMMENDED** generally; project policy may require it for high-impact or security-sensitive changes.
- **Observability Agent: OPTIONAL**; run telemetry can instead be owned by the harness or an existing platform.

See [Agent Model](docs/architecture/agent-model.md) for responsibilities and permission boundaries.

## AI-Assisted Delivery Lifecycle

Requirement → Specification → Planning → Context Discovery → Architecture Analysis → Implementation → Automated Validation → Tech Lead Review → bounded Correction Loop → Human Review when required → Delivery → Observability / Evaluation.

Each stage has an owner, expected evidence, and a stop/escalation condition. See [SDD](docs/sdd/README.md), [Tech Lead Review](docs/governance/tech-lead-review.md), and [AI Observability](docs/observability/ai-observability.md).

## Maturity Guide

1. **AI Assisted:** root instructions and a human-controlled implementation workflow.
2. **Context Driven:** architecture rules, ADRs, technology guidance, and minimum-relevant context selection.
3. **Spec Driven:** specifications, acceptance criteria, plans, tasks, and traceable validation.
4. **Tool Connected:** reviewed skills and least-privilege tools with explicit audit boundaries.
5. **Governed Agents:** independent technical review and defined human escalation.
6. **Harness Engineering:** privacy-conscious observability, evaluation, policy checks, and feedback loops.
7. **Agentic Engineering:** selected bounded autonomous workflows with human checkpoints and recovery.

Stages are adoption options, not a score or a destination. A small project may remain effective at an earlier stage.

## Structure

- `AGENT.md`: reusable project-root instruction template.
- `docs/architecture/`: harness, roles, and context strategy.
- `docs/sdd/`: specifications, requirements, acceptance, constraints, and planning templates.
- `docs/governance/`: review, permissions, security, escalation, and correction limits.
- `docs/mcp/` and `docs/rag/`: optional integration patterns.
- `docs/observability/`: trace model, metrics, and evaluation.
- `docs/adr/`: ADR template and proposed examples.
- `skills/`: skill contract and category guidance.
- `templates/`: operational feature, plan, review, and evaluation forms.

## Example Domain

Examples may use generic entities such as Customer, Order, Product, Payment, or Notification. Replace these with a reviewed domain vocabulary. Examples do not define production behavior.
