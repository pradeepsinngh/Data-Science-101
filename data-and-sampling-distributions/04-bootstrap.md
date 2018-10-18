## Bootstrap

One easy and effective way to estimate the sampling distribution of a statistic, or of model parameters, is to draw additional 
samples, with replacement, from the sample itself and recalculate the statistic or model for each resample. This procedure is 
called the bootstrap, and it does not necessarily involve any assumptions about the data or the sample statistic being normally
distributed.

- Bootstrap sample : A sample taken with replacement from an observed data set.
- Resampling : The process of taking repeated samples from observed data; includes both bootstrap and permutation (shuffling) 
procedures.

**Conceptually**, you can imagine the bootstrap as replicating the original sample thousands or millions of times so that you have a hypothetical population that embodies all the knowledge from your original sample (it’s just larger). You can then draw samples from this hypothetical population for the purpose of estimating a sampling distribution. 

The algorithm for a bootstrap resampling of the mean is as follows, for a sample of size n:

- Draw a sample value, record, replace it.
- Repeat n times.
- Record the mean of the n resampled values.
- Repeat steps 1–3 R times.
- Use the R results to:
  - Calculate their standard deviation (this estimates sample mean standard error).
  - Produce a histogram or boxplot.
  - Find a confidence interval.
  
- R, the number of iterations of the bootstrap, is set somewhat arbitrarily. 
- more iterations, the more accurate the estimate of the standard error, or the confidence interval. 
- The result from this procedure is a bootstrap set of sample statistics or estimated model parameters, which you can then examine to see how variable they are.

**Warning**
The bootstrap does not compensate for a small sample size; it does not create new data, nor does it fill in holes in an existing data set. It merely informs us about how lots of additional samples would behave when drawn from a population like our original sample.

## Resampling VS Bootstrapping

Sometimes the term resampling is used synonymously with the term bootstrapping. More often, the term resampling also includes permutation procedures, where multiple samples are combined and the sampling may be done without replacement. In any case, the term bootstrap always implies sampling with replacement from an observed data set.



### Key Ideas

1. The bootstrap (sampling with replacement from a data set) is a powerful tool for assessing the variability of a sample statistic.
2. The bootstrap can be applied in similar fashion in a wide variety of circumstances, without extensive study of mathematical approximations to sampling distributions.
3. It also allows us to estimate sampling distributions for statistics where no mathematical approximation has been developed.
4. When applied to predictive models, aggregating multiple bootstrap sample predictions (bagging) outperforms the use of a single model.


