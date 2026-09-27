# AI Metrics

**Classification: OPTIONAL instrumentation; metric definitions should be agreed before collection.**

Metrics describe populations of runs; traces explain individual execution. Define numerator, denominator, eligibility, exclusions, owner, sampling, and privacy treatment before publishing a rate. Do not create universal acceptable thresholds.

## Quality

- Specification compliance rate, based on criterion-level review.
- Architecture compliance rate and confirmed architecture violation rate.
- Required test/validation success rate.
- Tech Lead acceptance distribution across the four review statuses.
- Security finding rate and confirmed security violations.

## Autonomy

- First-pass success rate: eligible tasks accepted without a correction attempt.
- Self-correction success rate: blocking findings resolved by an agent correction and verified on re-review.
- Human intervention rate, segmented by trigger and task risk.
- Escalation appropriateness, sampled by human audit.

## Efficiency

- Input, output, and total tokens per run/task, when provider data is available.
- Context-size or context-budget utilization.
- Estimated cost per run/task with rate-card version and attribution caveats.
- Stage and total execution duration.
- Tool-call count, failed-call count, and retry count.
- Correction-loop attempts and time spent in correction.

## Reliability

- Failed, timed-out, cancelled, or denied tool calls.
- Failed validation runs and rerun rate.
- Architecture and security violation counts, severity-weighted only with a documented method.
- Correction-loop exhaustion and non-convergence.
- Review disagreement and false-positive/false-negative rates from human sampling.

## Targets

Set targets only after a project establishes a baseline, task mix, risk tolerance, data quality, and cost model. Revisit targets as models, prompts, tools, and scope change. Never reward a lower human-intervention rate if it discourages appropriate escalation.
