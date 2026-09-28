# Domain Discovery Skill

## Purpose
Recover domain concepts and business capabilities from a legacy codebase.

## Analyze
- entities and value-like objects
- services and use-case classes
- business rules visible in code
- terminology repeated across UI, application, data, and integration layers
- relationships between domain concepts

## Output
Prefer `docs/reverse-engineering/03-domain-model.md`.

## Guardrails
- do not expose real customer or production data
- distinguish business terminology from implementation terminology
- mark speculative domain boundaries as INFERRED
