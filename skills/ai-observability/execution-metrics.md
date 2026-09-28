# Execution Metrics Skill

## Purpose
Capture operational telemetry for agent workflows.

## Metrics
When available: duration, tool calls, tool failures, retries, correction attempts, context size, execution status, Tech Lead result, and human escalation/intervention.

## Rules
Use stable run/trace identifiers. Keep telemetry separate from prompt/source content. Report missing instrumentation explicitly. Do not infer tool failures, retries, or human intervention from token patterns.
