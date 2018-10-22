## Resampling

Resampling in statistics means to repeatedly sample values from observed data, with a general goal of assessing random variability in a statistic.

There are two main types of resampling procedures: 
- the bootstrap and 
- permutation tests. 

The bootstrap is used to assess the reliability of an estimate. Permutation tests are used to test hypotheses, typically involving two or more groups.

**Permutation test :** The procedure of combining two or more samples together, and randomly (or exhaustively) reallocating the observations to resamples. Also, called Randomization test, random permutation test, exact test.

**With or without replacement :** In sampling, whether or not an item is returned to the sample before the next draw.

## Permutation Test
- In a permutation test, two or more samples are involved, typically the groups in an A/B or other hypothesis test. 
- Permute means to change the order of a set of values. 
- The permutation procedure is as follows:
  - Combine the results from the different groups in a single data set.
  - Shuffle the combined data, then randomly draw (without replacing) a resample of the same size as group A.
  - From the remaining data, randomly draw (without replacing) a resample of the same size as group B.
  - Do the same for groups C, D, and so on.
  - Whatever statistic or estimate was calculated for the original samples (e.g., difference in group proportions), calculate it now for the resamples, and record; this constitutes one permutation iteration.
  - Repeat the previous steps R times to yield a permutation distribution of the test statistic.
  - Now go back to the observed difference between groups and compare it to the set of permuted differences. 
  - If the observed difference lies well within the set of permuted differences, then we have not proven anything.
  - However, if the observed difference lies outside most of the permutation distribution, then we conclude that chance is not responsible. In technical terms, the difference is statistically significant.
  
  

## Exhaustive and Bootstrap Permutation Test

There are two variants of the permutation test:
- An exhaustive permutation test
- A bootstrap permutation test

In an exhaustive permutation test, instead of just randomly shuffling and dividing the data, we actually figure out all the possible ways it could be divided. This is practical only for relatively small sample sizes. With a large number of repeated shufflings, the random permutation test results approximate those of the exhaustive permutation test, and approach them in the limit. Exhaustive permutation tests are also sometimes called exact tests, due to their statistical property of guaranteeing that the null model will not test as “significant” more than the alpha level of the test.

In a bootstrap permutation test, the draws outlined in the random permutation test are made with replacement instead of without replacement. In this way the resampling procedure models not just the random element in the assignment of treatment to subject, but also the random element in the selection of subjects from a population.


**KEY IDEAS**
- In a permutation test, multiple samples are combined, then shuffled.
- The shuffled values are then divided into resamples, and the statistic of interest is calculated.
- This process is then repeated, and the resampled statistic is tabulated.
- Comparing the observed value of the statistic to the resampled distribution allows you to judge whether an observed difference between samples might occur by chance.


