# Experiment Plan Template

## Experiment Details
- Experiment name:
- Experiment ID:
- Owner:
- Product / page / feature:
- Planned dates:
- Status: Draft / QA / Running / Complete

## Decision
What decision will change based on this experiment? What will be done after a win, loss, or inconclusive result?

## Context and Hypothesis
- Observation or evidence:
- Proposed change:
- Expected effect:
- Target audience:
- Primary metric:

> Because [observation], we believe [change] will cause [expected outcome] for [audience]. We will evaluate this using [metric and decision threshold].

## Experiment Design
- Type: A/B / A/B/n / Multivariate / Split URL
- Randomization unit:
- Assignment method:
- Eligibility and exclusions:
- Variant persistence:
- Traffic allocation:

| Variant | Description | Difference from control | QA |
|---|---|---|---|
| A (control) | Current experience | None | |
| B (treatment) | Proposed experience | | |

## Metrics
| Class | Metric | Exact definition | Data source |
|---|---|---|---|
| Primary | | | |
| Secondary | | | |
| Guardrail | | | |

Define event names, numerator, denominator, attribution window, and reporting unit.

## Statistical Plan
- Baseline:
- Minimum detectable effect:
- Significance level:
- Target power:
- Required sample per variant:
- Eligible traffic estimate:
- Planned duration:
- Multiplicity method:
- Stopping rule:

## Implementation and QA
- Client-side / server-side:
- Experiment platform:
- Assignment event:
- Exposure event:
- Outcome event:
- Sample-ratio mismatch check:
- QA owner:
- Performance or flicker risk:

## Risks and Sign-off
- User, revenue, reliability, privacy, or operational risks:
- Guardrail thresholds:
- Rollback owner:
- Approvers:
- [ ] Hypothesis and decision are clear.
- [ ] Metrics and events are approved.
- [ ] Sample size and stopping rules are set.
- [ ] Variants and tracking are verified.
- [ ] Analysis plan is saved before launch.
