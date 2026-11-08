# claude-ab-test-setup-skill

A Claude Code skill for planning, designing, implementing, and evaluating A/B tests and product experiments.

## Overview

This skill helps design experiments that produce interpretable and actionable results. It covers hypothesis formation, baseline measurement, success metrics, sample size considerations, variant design, implementation, and analysis.

A test should be run only when the team can define what decision the result will inform.

## Main Capabilities

- Clarify the business or product question.
- Form a measurable hypothesis.
- Define control and treatment variants.
- Select primary and guardrail metrics.
- Assess baseline conversion and traffic volume.
- Plan experiment duration and sample size.
- Identify segmentation and randomization requirements.
- Implement experiment assignment and exposure tracking.
- Analyze results and uncertainty.
- Document decisions and follow-up actions.

## Initial Assessment

Before designing the test, establish:

- What outcome should improve?
- What change is being tested?
- What is the current baseline?
- How much eligible traffic is available?
- Which metrics define success?
- What guardrails must not deteriorate?
- What technical and timeline constraints exist?

## Installation

```bash
git clone https://github.com/Brajesh31/claude-ab-test-setup-skill.git ~/.claude/skills/ab-test-setup
```

## Usage

Invoke the skill when planning an experiment:

```text
/ab-test-setup
```

Provide the product change, audience, baseline metric, expected effect, traffic volume, and experiment platform.

## Experiment Plan Structure

| Element | Description |
|---|---|
| Objective | Decision the experiment supports |
| Hypothesis | Expected measurable effect |
| Control | Current experience |
| Treatment | Proposed change |
| Primary metric | Main success measure |
| Guardrail metrics | Measures that must remain healthy |
| Audience | Eligible population |
| Assignment | Randomization method |
| Duration | Planned exposure period |
| Decision rule | Criteria for interpreting results |

## Recommended Workflow

1. Define the decision and hypothesis.
2. Confirm that the metric can be measured reliably.
3. Review baseline conversion and traffic.
4. Estimate sample size and experiment duration.
5. Define variants and assignment logic.
6. Implement exposure and outcome tracking.
7. Test assignment, event collection, and sample-ratio balance.
8. Run the experiment without repeatedly changing the decision rule.
9. Analyze the result with uncertainty and practical effect size.
10. Decide whether to ship, iterate, or stop.

## Analysis Considerations

- Avoid peeking and stopping solely because a temporary result looks favorable.
- Check sample-ratio mismatch.
- Consider novelty and seasonality effects.
- Watch for multiple comparisons.
- Keep the unit of randomization consistent.
- Distinguish statistical significance from practical value.
- Review guardrail metrics before rollout.
- Document limitations and unexpected effects.

## Repository Contents

- `SKILL.md`: Main experiment design and analysis instructions.
- `README.md`: Planning workflow and experiment checklist.

## Quality Checklist

- Hypothesis is specific and falsifiable.
- Primary metric is defined before launch.
- Baseline data is trustworthy.
- Assignment is randomized and consistent.
- Exposure events are recorded correctly.
- Sample size is sufficient for the expected effect.
- Guardrail metrics are monitored.
- Analysis accounts for uncertainty.
- Decision and limitations are documented.

## Practical Principle

If traffic is too low or the expected effect is too small to measure, do not pretend the test can produce a reliable answer. Consider a qualitative study, staged rollout, or another evaluation method.
