# Requirements Template

> **TEMPLATE:** Assign stable identifiers. Requirements must be specific enough to validate without prescribing an implementation unnecessarily.

## Functional Requirements

| ID | Requirement statement | Priority | Source / rationale | Verification |
| --- | --- | --- | --- | --- |
| `FR-001` | The system shall `[observable behavior]` when `[condition]`. | `[MUST/SHOULD/MAY]` | `[SOURCE]` | `[TEST OR REVIEW]` |

## Non-Functional Requirements

| ID | Quality attribute | Requirement / target | Measurement method | Owner / status |
| --- | --- | --- | --- | --- |
| `NFR-001` | `[SECURITY/PERFORMANCE/RELIABILITY/ACCESSIBILITY/PRIVACY]` | `[PROJECT-DEFINED TARGET]` | `[HOW MEASURED]` | `[OWNER / OPEN]` |

Do not invent universal availability, latency, coverage, cost, or quality thresholds. Targets require project context, measurement definitions, and an accountable owner.

## Constraints

- **Policy:** `[SECURITY_OR_LEGAL_RULES]`
- **Architecture:** `[BOUNDARIES_OR_ADRS]`
- **Compatibility:** `[PUBLIC_CONTRACTS_OR_CLIENTS]`
- **Data:** `[CLASSIFICATION_AND_RETENTION]`
- **Operations:** `[DEPLOYMENT_OR_RECOVERY_CONSTRAINTS]`

## Requirement Quality Check

- One requirement expresses one outcome.
- Wording is observable and testable.
- Priority and source are known.
- Ambiguity is tracked as a question, not hidden in implementation.
- Security, privacy, and authorization impact are identified.
- Verification method is named before delivery.
