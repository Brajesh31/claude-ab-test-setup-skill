# Statistical Interpretation Notes

These notes supplement the skill's experiment workflow. A favorable result can still be misleading when assignment, measurement, or stopping rules are invalid.

## P-values
A p-value is the probability, assuming the null hypothesis and statistical model are true, of observing data at least as extreme as the data obtained. It is not the probability that the result is random or that the null hypothesis is true.

A threshold such as 0.05 is a convention under specified assumptions. It does not replace effect-size estimation or business judgment.

## Confidence Intervals
A confidence interval is produced by a procedure that, under its assumptions, covers the true parameter at its stated rate over repeated samples. A 95% confidence interval is not ordinarily interpreted as a 95% probability that this one computed interval contains the fixed true value.

Report the interval and explain the range of effects compatible with the data.

## Power and Sample Size
Required sample size depends on the baseline, variance or conversion rate, MDE, significance level, target power, number of arms, allocation, randomization unit, clustering, and attrition. Recalculate for the actual design rather than reusing a generic table.

## Repeated Peeking
Repeatedly checking ordinary fixed-horizon p-values and stopping when one becomes favorable inflates false-positive risk. Pre-specify the sample size and stopping time, or use a valid sequential design.

## Multiple Comparisons
Testing many metrics, variants, or subgroups increases the chance of a spurious positive. Define one primary metric, pre-plan important segments, and apply an appropriate multiplicity strategy to multiple confirmatory claims.

## Statistical and Practical Significance
A small effect can be statistically detectable with large traffic but not worth implementation cost. Interpret magnitude, uncertainty, cost, and guardrails together.

## Minimum Reporting Standard
Report the design, randomization unit, sample sizes, metric definitions, effect estimate, uncertainty interval, stopping rule, guardrail results, deviations, and decision. Never call an underpowered or invalid experiment a clean win.
