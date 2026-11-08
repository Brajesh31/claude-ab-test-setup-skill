# A/B Experiment Pre-Launch Checklist

## Design
- [ ] Decision supported by the experiment is explicit.
- [ ] Hypothesis is specific and falsifiable.
- [ ] Primary metric is selected before launch.
- [ ] Secondary and guardrail metrics are defined.
- [ ] Eligibility and exclusion rules are documented.
- [ ] Randomization unit matches the analysis unit.
- [ ] Sample size, power, MDE, and stopping rule are documented.
- [ ] Important segments are planned in advance.

## Implementation
- [ ] Assignment is random and stable for returning users where required.
- [ ] Control and treatment are implemented correctly.
- [ ] Exposure is recorded only when the variant is actually shown.
- [ ] Outcome events are deduplicated and validated.
- [ ] Cross-device behavior is understood.
- [ ] Flicker, latency, and feature-flag behavior are checked.

## Data Quality
- [ ] Event names and properties are correct.
- [ ] Denominators and attribution windows are explicit.
- [ ] Sample-ratio mismatch checks are configured.
- [ ] Bots and internal traffic are treated consistently.
- [ ] Dashboards and data pipelines are available.
- [ ] Instrumentation is tested before the experiment begins.

## Governance
- [ ] Stakeholders understand the decision rule.
- [ ] The team will not stop early on a favorable dashboard snapshot.
- [ ] Rollback owner and guardrail thresholds are documented.
- [ ] Privacy and consent requirements are satisfied.
- [ ] Plan and analysis method are saved before launch.

Do not launch while critical assignment, tracking, privacy, or safety issues remain unresolved.
