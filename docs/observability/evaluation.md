# AI Evaluation

**Classification: CORE to define evaluation criteria; a persistent evaluation platform is OPTIONAL.**

Evaluation checks whether the harness and agents behave as intended across representative tasks. It complements deterministic tests and human review; it does not replace either.

## Evaluation Dimensions

- **Quality:** specification compliance, architecture compliance, test outcomes, review acceptance, correctness, and completeness.
- **Autonomy:** first-pass success, self-correction success, appropriate escalation, and human intervention rate.
- **Efficiency:** tokens, estimated cost, duration, tool calls, and retries per eligible task.
- **Reliability:** failed tool calls, repeated failures, architecture/security violations, and correction-loop exhaustion.
- **Safety:** secret/data handling, authorization denial, privileged-action approval, prompt-injection resistance, and uncertainty reporting.

## Evaluation Set

Use versioned, synthetic tasks representing routine work, requirement ambiguity, architecture boundaries, security-sensitive changes, tool failure, conflicting instructions, and prohibited actions. Define expected behavior and unacceptable outcomes. Keep task data free of real user/customer content unless separately approved.

## Evaluation Process

1. Establish a baseline for a fixed model/prompt/tool/policy version.
2. Run repeatable tests when any of those components changes.
3. Compare outcome metrics with confidence and task-type segmentation.
4. Have humans inspect safety failures, high-impact decisions, and a representative sample.
5. Block rollout on project-defined critical regressions; document accepted limitations.

Targets and thresholds are project-specific. Do not invent universal pass rates or optimize one score at the expense of correctness, security, or appropriate escalation.
