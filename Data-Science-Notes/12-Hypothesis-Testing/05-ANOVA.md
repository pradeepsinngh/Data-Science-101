## ANOVA - analysis of variance

Suppose that, instead of an A/B test, we had a comparison of multiple groups, say A-B-C-D, each with numeric data. The 
statistical procedure that tests for a statistically significant difference among the groups is called analysis of variance, or ANOVA.


**Key Terms**

- Pairwise comparison : A hypothesis test (e.g., of means) between two groups among multiple groups.
- Omnibus test : A single hypothesis test of the overall variance among multiple group means.
- Decomposition of variance : Separation of components. contributing to an individual value (e.g., from the overall average, from a treatment mean, and from a residual error).
- F-statistic : A standardized statistic that measures the extent to which differences among group means exceeds what might be expected in a chance model.
- SS : “Sum of squares,” referring to deviations from some average value.

## F-Statistic

- Just like the t-test can be used instead of a permutation test for comparing the mean of two groups, there is a statistical test for ANOVA based on the F-statistic.
- The F-statistic is based on the ratio of the variance across group means (i.e., the treatment effect) to the variance due to residual error. 
- The higher this ratio, the more statistically significant the result. If the data follows a normal distribution, then statistical theory dictates that the statistic should have a certain distribution. Based on this, it is possible to compute a p-value.



## Two-Way ANOVA

- The A-B-C-D test just described is a “one-way” ANOVA, in which we have one factor (group) that is varying. 
- We could have a second factor involved—say, “weekend versus weekday”—with data collected on each combination (group A weekend, group A weekday, group B weekend, etc.) and this would be a “two-way ANOVA,”. 

You can see that ANOVA, then two-way ANOVA, are the first steps on the road toward a full statistical model, such as regression and logistic regression, in which multiple factors and their effects can be modeled.

**Key Ideas**

- ANOVA is a statistical proecdure for analyzing the results of an experiment with multiple groups.
- It is the extension of similar procedures for the A/B test, used to assess whether the overall variation among groups is within the range of chance variation.
- A useful outcome of an ANOVA is the identification of variance components associated with group treatments, interaction effects, and errors.

