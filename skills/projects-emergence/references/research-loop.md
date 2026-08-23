# Proportionate research loop

Read this reference when a decision needs evidence beyond existing project context or a direct verification.

## Route by decision risk

| Situation | Default approach | Typical budget |
|---|---|---:|
| New problem definition, audience, or core hypothesis | Full research loop | 30–45 minutes |
| Reference mechanism, architecture, or competing designs | Focused research loop | 20–30 minutes |
| Familiar API or ordinary implementation detail | Official documentation or direct verification | 5–10 minutes |
| Bug or regression with an unclear cause | Diagnosis and minimal reproduction | 15–30 minutes |
| Publishing, migration, privacy, data, cost, or external service | Risk check | 20–40 minutes |
| Known mechanical work with clear acceptance criteria | No separate research loop | 0 minutes |

Budgets are upper bounds, not quotas.

## Minimum loop

1. **Define the decision.** State the one action the research must support.
2. **State the current hypothesis.** Name the most likely explanation or option before searching.
3. **Collect the minimum evidence set.** Start with one primary or official source. Add sources only for conflicts, risk, or missing boundaries.
4. **Verify.** Use a reproduction, test, log, version check, comparison, or small experiment.
5. **Replay the result.** Report evidence, conclusion, confidence, next action, and unresolved risk.
6. **Stop or escalate.** Stop when the next decision is supported. Escalate only when evidence conflicts or the impact is larger than expected.

## Evidence cards

During interactive research, keep each update small:

```text
Question: What decision are we supporting?
Evidence:
- Source or observation: what it supports
- Source or observation: what it does not establish
Current judgment: provisional conclusion and confidence
Next decision: one choice or correction needed
```

Search summaries are discovery aids, not final evidence. Prefer official documentation, primary research, source repositories, issues, and direct experiments.

For a reusable source record, capture:

- title and author or maintainer;
- URL and access date;
- license when reuse is possible;
- observed mechanism;
- reproducible boundary;
- evidence strength and remaining uncertainty.

## Research gate replay

Before implementation, summarize:

```text
Problem:
Reference mechanism:
Evidence:
Uncertainty:
Chosen path: replicate / adapt / improve / redesign
Smallest implementation:
Verification:
Public/private boundary:
Confirmation needed:
```

## Stop conditions

Stop researching when any of these is true:

- one reliable source plus direct verification supports the decision;
- new sources repeat known information without changing the choice;
- two viable options and their tradeoffs are clear;
- a test or minimal reproduction can answer the question faster;
- the time budget is exhausted and the remaining uncertainty is recorded.

Increase the budget only for conflicting evidence, security, privacy, data loss, meaningful cost, public impact, unstable reproduction, or a hard-to-reverse decision. If a second budget still produces no conclusion, state what remains unknown and propose a smaller experiment.
