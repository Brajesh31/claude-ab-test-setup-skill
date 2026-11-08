# A/B Test Setup Skill

A practical skill for planning, launching, monitoring, and evaluating controlled product and marketing experiments. It focuses on clear hypotheses, measurable outcomes, valid experiment design, reliable assignment, and decisions grounded in both statistical and business significance.

## What This Skill Helps With

- Turn an observation into a falsifiable hypothesis.
- Choose between A/B, A/B/n, multivariate, and split-URL experiments.
- Define control and treatment variants.
- Select primary, secondary, and guardrail metrics.
- Estimate sample size and experiment duration.
- Choose client-side or server-side implementation.
- Validate assignment and exposure tracking.
- Monitor experiment quality without changing decision rules.
- Interpret results and record follow-up actions.

## When to Use It

Use this skill for controlled experiments, product changes, page variants, conversion optimization, copy or design tests, and experiment documentation. It is not a substitute for a testing platform or statistical review. Result quality depends on valid assignment, reliable instrumentation, enough sample, and a suitable analysis method.

## Installation

~~~bash
git clone https://github.com/Brajesh31/claude-ab-test-setup-skill.git ~/.claude/skills/ab-test-setup
~~~

## Usage

Invoke:

~~~text
/ab-test-setup
~~~

Provide the product change, target audience, baseline, expected effect, traffic volume, event definitions, test platform, and the decision the experiment should support.

## Experiment Design Workflow

1. Define the decision and the observation that motivates the test.
2. Write a falsifiable hypothesis with an expected direction and metric.
3. Choose the simplest design that answers the question.
4. Define one primary metric plus secondary and guardrail metrics.
5. Estimate sample size and duration from the actual experiment assumptions.
6. Define eligibility, exclusions, randomization unit, and variant persistence.
7. Validate assignment, exposure, and outcome events before launch.
8. Pre-specify the stopping rule and analysis method.
9. Monitor technical health and data quality while the test runs.
10. Analyze effect size, uncertainty, practical value, and guardrails.
11. Record the decision and follow-up learning.

## Core Documents

| Document | Purpose |
|---|---|
| Experiment plan | Captures hypothesis, variants, metrics, sample size, and analysis |
| Pre-launch checklist | Confirms assignment, tracking, QA, and guardrails |
| Results review | Records outcomes, uncertainty, limitations, and decision |
| Statistical notes | Explains p-values, intervals, power, and repeated peeking |

## Included Resources

- [Experiment plan template](resources/experiment-plan-template.md)
- [Pre-launch checklist](resources/pre-launch-checklist.md)
- [Results review template](resources/results-review-template.md)
- [Statistical interpretation notes](resources/statistical-interpretation.md)

## Statistical Caution

A p-value is not the probability that a result is random or that the null hypothesis is true. A 95% confidence procedure does not imply a 95% probability that this particular interval contains the fixed true value. Report effect estimates and uncertainty, and distinguish statistical detectability from practical value.

## Quality Checklist

- The primary metric is defined before launch.
- The randomization unit matches the analysis unit.
- Assignment is stable where needed.
- Exposure and outcome events are verified.
- Sample size and stopping rules are documented.
- Sample-ratio mismatch and instrumentation issues are checked.
- Multiple comparisons and post-hoc segments are handled carefully.
- Guardrails are reviewed before rollout.
- Inconclusive results are reported honestly.

## Repository Structure

~~~text
claude-ab-test-setup-skill/
├── SKILL.md
├── README.md
├── LICENSE
└── resources/
    ├── experiment-plan-template.md
    ├── pre-launch-checklist.md
    ├── results-review-template.md
    └── statistical-interpretation.md
~~~

## License

See LICENSE. The source skill's MIT notice is preserved, with a separate notice for newly written repository documentation.
