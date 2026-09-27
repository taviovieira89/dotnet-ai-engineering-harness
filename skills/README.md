# Skills Architecture

**Classification: CORE to define a skill contract; individual skills are OPTIONAL.**

A skill is a versioned instructional package for a repeatable task domain. It may define procedures, required context, expected outputs, and validation. It does not grant tools or permissions. The harness must enforce access independently.

## Suggested Structure

```text
skills/
├── frontend/
├── backend/
├── architecture/
├── testing/
├── security/
├── devops/
├── integrations/
└── observability/
```

Each category can contain one or more task-scoped `SKILL.md` files using [SKILL-TEMPLATE.md](SKILL-TEMPLATE.md). Do not create placeholder skills just to fill the tree.

## Skill Lifecycle

Define an owner and invocation criteria; review inputs, permissions, and validation; test for instruction conflicts and unsafe tool assumptions; version changes; and retire stale skills. Keep examples generic and mark them as examples.

## Categories

- [Frontend](frontend/README.md)
- [Backend](backend/README.md)
- [Architecture](architecture/README.md)
- [Testing](testing/README.md)
- [Security](security/README.md)
- [DevOps](devops/README.md)
- [Integrations](integrations/README.md)
- [Observability](observability/README.md)
