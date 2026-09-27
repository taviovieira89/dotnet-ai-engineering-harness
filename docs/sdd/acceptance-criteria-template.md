# Acceptance Criteria Template

> **TEMPLATE:** Define externally observable behavior. Keep criteria independent of implementation details unless a technical constraint is intentional.

## Acceptance Criteria

| ID | Given | When | Then | Verification evidence |
| --- | --- | --- | --- | --- |
| `AC-001` | `[PRECONDITION]` | `[ACTION]` | `[OBSERVABLE RESULT]` | `[TEST / REVIEW]` |

## Required Case Categories

Select the categories applicable to the feature:

- Expected success and boundary values.
- Invalid or incomplete input.
- Unauthorized actor or out-of-scope resource.
- Conflict, concurrency, or duplicate request.
- Dependency failure, timeout, or partial result.
- Retry, recovery, cancellation, and idempotency.
- Privacy, logging, and sensitive-data handling.
- Accessibility and user-visible error state.

## Generic Example (Illustrative Only)

- **Given** an authorized user viewing an order they may access,
- **When** they request the order's current status,
- **Then** the system returns the status and a correlation reference, without exposing data outside the user's scope.

This example demonstrates testable phrasing only. It does not define a project's authorization policy or data model.

## Review Checklist

- Each criterion can be verified as pass/fail.
- Error and negative behavior are explicit.
- Required roles and data scope are named without embedding secrets or real personal data.
- Tests can trace back to criterion IDs.
- The accountable domain owner has approved business semantics.
