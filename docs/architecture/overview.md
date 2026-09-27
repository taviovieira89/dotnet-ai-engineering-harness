# Architecture Overview

## Classification

CORE TEMPLATE

## Purpose

The AI Engineering Harness is the controlled environment around one or more language models and agents. It supplies authoritative instructions, minimum task context, bounded tools, validation, independent review, human approval paths, and execution evidence.

It is not a specific model, a single agent prompt, or a guarantee of correctness. A project should adopt the smallest architecture that meets its risk and delivery needs.

## Logical Layers

| Layer | Responsibility |
| --- | --- |
| Policy | Security, privacy, data classification, approval, and non-negotiable constraints. |
| Context | Assemble task-relevant instructions, specifications, architecture, ADRs, skills, code, and knowledge. |
| Orchestration | Assign roles, sequence stages, bound retries, and preserve run identity. |
| Agent | Plan, implement, review, or observe within role and permission limits. |
| Tool boundary | Expose task-scoped repository, validation, and optional external capabilities. |
| Validation | Run deterministic checks and collect results as evidence. |
| Governance | Route review outcomes, correction, human decisions, and delivery. |
| Observability | Capture privacy-minimized execution and quality metadata. |

## CORE

- One authoritative project instruction entry point.
- Requirements and acceptance criteria before substantial implementation.
- Explicit architecture rules and ADR status.
- Least-privilege read/write/privileged access.
- Automated validation and honest reporting of unrun checks.
- Human escalation for reserved or uncertain decisions.
- A Definition of Done that includes specification, security, tests, review, and required approvals.

## OPTIONAL

Separate planning/review/observability agents, MCP, RAG, multiple models, vector search, external ticket/pipeline integrations, and bounded automated correction. Adopt only with a use case, owner, threat review, evaluation, and rollback plan.

## Technology and Domain Configuration

This template does not prescribe a language, frontend framework, database, cloud, model provider, or domain. Record selected technologies and boundaries in project-specific guidelines and ADRs. Use generic examples only until a real domain is approved.

See [AI Harness](ai-harness.md), [Agent Model](agent-model.md), and [Context Engineering](context-engineering.md).
