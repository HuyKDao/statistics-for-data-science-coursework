# Hypothesis Testing & Statistical Power

**Course:** ESE 5420, Statistics for Data Science (University of Pennsylvania, Spring 2026), Homework 6–7

**Question:** When is a result strong enough to act on, and how likely is a test to detect a real effect?

## What I did
- **z-tests and t-tests:** chose the right test for known vs. unknown variance, computed test statistics and decision rules at different significance levels, and turned a test's acceptance region into a matching confidence interval.
- **One-sided proportion test:** tested whether more than half of homes built with a certain material had electrical or environmental problems, and computed a one-sided lower confidence bound. I noted why the test uses the null proportion for its standard error while the interval uses the sample proportion.
- **p-values:** computed one- and two-sided p-values for a proportion test and interpreted the decisions at α = 0.05 and α = 0.01.
- **Power analysis in Python:** plotted **power curves** to show how a test's ability to detect an effect changes with the true mean, the significance level α, the sample size n and the noise variance σ².
- **Likelihood ratio test:** derived a generalized likelihood ratio test for the rate of an exponential distribution and showed the form of its rejection region.

## What I learned
- Power is the number to check before running an experiment: bigger samples and less noise buy detection, and a stricter α costs power.
- The same math underlies hypothesis tests and confidence intervals, which is why A/B test results can be read either way.

## Skills and tools
Hypothesis testing (z-test, t-test, one- and two-sided), p-values, significance levels, Type I and Type II error, power curves, likelihood ratio tests, Python, SciPy, NumPy, Matplotlib.
