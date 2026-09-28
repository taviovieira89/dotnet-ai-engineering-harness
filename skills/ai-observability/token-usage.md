# Token Usage Skill

## Purpose
Normalize provider/runtime token telemetry without inventing unavailable categories.

## Capture
When exposed, capture input, output, total, cached, and reasoning tokens using the provider's semantics.

## Rules
- Never infer hidden reasoning usage.
- Never treat unavailable as zero.
- Attribute usage to an agent/phase only when the runtime supports that attribution.
- For Plan Mode, use phase=PLAN rather than inventing a plan-token category.
- Preserve provider-specific fields when useful and map them separately to normalized fields.
