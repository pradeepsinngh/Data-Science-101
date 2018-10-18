## Sampling Distribution of a Statistic

The term sampling distribution of a statistic refers to the distribution of some sample statistic, over many samples drawn 
from the same population. Much of classical statistics is concerned with making inferences from (small) samples to 
(very large) populations.


- Sample statistic : A metric calculated for a sample of data drawn from a larger population.
- Data distribution : The frequency distribution of individual values in a data set.
- Sampling distribution : The frequency distribution of a sample statistic over many samples or resamples.
- Central limit theorem : The tendency of the sampling distribution to take on a normal shape as sample size rises.
- Standard error : The variability (standard deviation) of a sample statistic over many samples (not to be confused with standard deviation, which, by itself, refers to variability of individual data values).

## Philosophy:
Typically, a sample is drawn with the goal of measuring something (with a sample statistic) or modeling something (with a statistical or machine learning model). Since our estimate or model is based on a sample, it might be in error; it might be different if we were to draw a different sample. We are therefore interested in how different it might be—a key concern is sampling variability. If we had lots of data, we could draw additional samples and observe the distribution of a sample statistic directly. Typically, we will calculate our estimate or model using as much data as is easily available, so the option of drawing additional samples from the population is not readily available.

**NOTE:** The distribution of the individual data points is known as the data distribution, and the distribution of a sample statistic is known as the sampling distribution.

**NOTE:** 
1. The distribution of a sample statistic such as the mean is likely to be more regular and bell-shaped than the distribution of the data itself. 
2. The larger the sample that the statistic is based on, the more this is true. Also, the larger the sample, the narrower the distribution of the sample statistic.


## Central Limit Theorem
It says that the means drawn from multiple samples will resemble the familiar bell-shaped normal curve, even if the source population is not normally distributed, provided that the sample size is large enough and the departure of the data from normality is not too great. 

## Standard Error
1. The standard error is a single metric that sums up the variability in the sampling distribution for a statistic.
2. The standard error can be estimated using a statistic based on the standard deviation s of the sample values, and the sample size n: SE = s/sqrt(n)
3. As the sample size increases, the standard error decreases. 
4. The relationship between standard error and sample size is sometimes referred to as the square-root of n rule: in order to reduce the standard error by a factor of 2, the sample size must be increased by a factor of 4.


**NOTE:--** 
### Standard Deviation versus Standard Error
Do not confuse standard deviation (which measures the variability of individual data points) with standard error (which measures the variability of a sample metric).

