---
name: [generic-skill-name]
description: [When this skill should be selected]
owner: [accountable-role]
version: [version]
---

# [Skill Name]

> **TEMPLATE:** This file defines knowledge and workflow. It does not authorize tools or override project instructions.

## Purpose

[Problem this skill helps solve and intended users/agents.]

## Responsibility

[What the skill covers and what remains outside its scope.]

## Inputs

- `[task specification or request]`
- `[required artifacts, code, and evidence]`
- `[data classification and assumptions]`

## Outputs

- `[expected artifact, decision, or validation evidence]`
- `[required format and provenance]`

## Allowed Tools

- `[tool category and permitted operation]`
- If none, state `None`.

Tool availability is separately controlled by the harness. Do not put credentials or private endpoints here.

## Required Context

- `[authoritative instructions and policies]`
- `[relevant architecture, ADR, or specification]`
- `[minimum code/test context]`

## Permissions

- **Read:** `[scope]`
- **Write:** `[scope or none]`
- **Privileged:** `[scope or none; human approval requirement]`
- **External systems:** `[scope or none]`

## Restrictions

- `[prohibited actions, assumptions, and data handling]`
- State explicitly that the skill itself does not grant permissions.

## Validation

- `[checks, expected evidence, and failure handling]`

## Human Approval Requirements

- `[triggers and accountable role; or none with rationale]`

## Examples

Use generic, synthetic examples only. Label them **EXAMPLE** and do not present them as approved policy.
