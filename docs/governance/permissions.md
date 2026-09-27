# Permission Model

**Classification: CORE.**

Permissions belong to the harness/tool layer. Agent instructions and skills describe intended behavior but must not be treated as enforcement. Grant the narrowest capability, resource, data scope, and duration needed for a task.

| Tier | Typical actions | Default policy |
| --- | --- | --- |
| `READ` | Read approved source, documentation, specifications, test/build results, and scoped work records. | Allow only relevant paths/data; classify and redact before model exposure. |
| `WRITE` | Modify scoped source, tests, documentation, or explicitly approved work items. | Require task authorization, allowed-path or resource scope, diff review, and audit record. |
| `PRIVILEGED` | Modify pipelines/infrastructure, deploy, access production, manage secrets, change permissions, or perform destructive actions. | Deny by default; require explicit policy, human approval, time-bound grant, and recovery/audit plan. |

## Permission Checks

For each tool call, verify agent identity/role, task intent, resource scope, data classification, operation type, approval requirement, and grant expiry. Re-check authorization at execution time; do not rely on model-supplied claims.

## Generic Capability Examples

- `READ`: repository code, docs, user-requested records, and build/test results.
- `WRITE`: task-scoped code/tests/docs; work-item writes only where separately authorized.
- `PRIVILEGED`: pipeline changes, infrastructure changes, deployment, production access, secret management, destructive operations.

## Audit

Record actor/agent, task/run ID, tool and operation category, target scope, approval reference where applicable, time, outcome, and correlation reference. Avoid recording credentials, full private content, or sensitive arguments.

See [MCP Strategy](../mcp/mcp-strategy.md): connecting a tool protocol does not expand this permission model.
