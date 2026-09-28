# Repository Inventory Skill

## Purpose
Create an evidence-based inventory of a legacy repository before architectural conclusions are made.

## Responsibilities
- identify solutions and projects
- identify application types and runtime/framework versions
- locate entry points and configuration
- identify tests and infrastructure artifacts
- identify dependency manifests
- identify existing documentation

## Output
Prefer `docs/reverse-engineering/00-system-inventory.md`.

## Guardrails
- read-only analysis
- do not infer runtime behavior without evidence
- do not expose secrets or environment-specific values
- classify findings as OBSERVED, INFERRED, or UNKNOWN
