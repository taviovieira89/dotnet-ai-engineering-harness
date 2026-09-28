# Implementation Review Skill

## Purpose
Review a code change against approved scope, specification, architecture, ADRs, implementation plan, and Definition of Done.

## Checks
- Map changed behavior to requirements.
- Detect unapproved scope expansion.
- Validate dependency and module boundaries.
- Review correctness, validation, error handling, resource ownership, async/cancellation/concurrency where relevant.
- Identify breaking API/data contracts.
- Verify required tests and operational instrumentation are present.
- Separate correctness/architecture findings from stylistic preferences.

## Output
Return evidence-based findings. Never modify the implementation as part of the review.
