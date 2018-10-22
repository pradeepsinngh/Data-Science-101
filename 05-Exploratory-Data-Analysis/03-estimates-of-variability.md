## Estimates of Variability:

- Location is just one dimension in summarizing a feature. 
- A second dimension, variability, measures whether the data values are tightly clustered or spread out. 
- At the heart of statistics lies variability: measuring it, reducing it, distinguishing random from real variability, 
identifying the various sources of real variability, and making decisions in the presence of it.


1. Deviations : The difference between the observed values and the estimate of location.
   - Synonyms : errors, residuals
2. Variance : The sum of squared deviations from the mean divided by n – 1 where n is the number of data values.
   - Synonyms : mean-squared-error
3. Standard deviation : The square root of the variance.
   - Synonyms : l2-norm, Euclidean norm
4. Mean absolute deviation : The mean of the absolute value of the deviations from the mean.
   - Synonyms : l1-norm, Manhattan norm
5. Median absolute deviation from the median : The median of the absolute value of the deviations from the median.
6. Range : The difference between the largest and the smallest value in a data set.
7. Order statistics : Metrics based on the data values sorted from smallest to biggest.
   - Synonyms : ranks
8. Percentile : The value such that P percent of the values take on this value or less and (100–P) percent take on this value or more.
   - Synonyms : quantile
9. Interquartile range : The difference between the 75th percentile and the 25th percentile.
   - Synonyms : IQR

## Standard Deviation and Related Estimates:

1. Mean Absolute deviation

best-known estimates for variability are the variance and the standard deviation, 
2. Variance:
3. Std. Deviation: 
   - The standard deviation is much easier to interpret than the variance since it is on the same scale as the original data. 
   - standard deviation is preferred in statistics over the mean absolute deviation because working with squared values is 
   much more convenient than absolute values, especially for statistical models.
   
 ## Why we have n – 1 in the denominator in the variance formula, instead of n?  
 ## Degrees of Freedom, and n or n – 1?
 - Why we have n – 1 in the denominator in the variance formula, instead of n, leading into the concept of degrees of freedom. 
 - This distinction is not important since n is generally large enough that it won’t make much difference whether you divide by n or n – 1.
 - But in case you are interested, **here is the story**. It is based on the premise that you want to make estimates about a population, based on a sample.
 
 If you use the intuitive denominator of n in the variance formula, you will underestimate the true value of the variance and the standard deviation in the population. This is referred to as a biased estimate. However, if you divide by n – 1 instead of n, the standard deviation becomes an unbiased estimate.

To fully explain why using n leads to a biased estimate involves the notion of degrees of freedom, which takes into account the number of constraints in computing an estimate. In this case, there are n – 1 degrees of freedom since there is one constraint: the standard deviation depends on calculating the sample mean. For many problems, data scientists do not need to worry about degrees of freedom, but there are cases where the concept is important (see “Choosing K”).

### What to choose?
- Neither the variance, the standard deviation, nor the mean absolute deviation is robust to outliers and extreme values.
- The variance and standard deviation are especially sensitive to outliers since they are based on the squared deviations.

- A robust estimate of variability is the **median absolute deviation from the median or MAD**:
