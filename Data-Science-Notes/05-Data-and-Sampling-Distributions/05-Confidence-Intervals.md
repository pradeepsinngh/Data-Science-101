## Confidence Intervals

Frequency tables, histograms, boxplots, and standard errors are all ways to understand the potential error in a sample 
estimate. Confidence intervals are another.


### Key Terms
- Confidence level : The percentage of confidence intervals, constructed in the same way from the same population, expected to contain the statistic of interest.
- Interval endpoints : The top and bottom of the confidence interval.

Confidence intervals always come with a coverage level, expressed as a (high) percentage, say 90% or 95%. One way to think of 
a 90% confidence interval is as follows: it is the interval that encloses the central 90% of the bootstrap sampling 
distribution of a sample statistic. More generally, an x% confidence interval around a sample estimate should, on average, 
contain similar sample estimates x% of the time (when a similar sampling procedure is followed).


Given a sample of size n, and a sample statistic of interest, the algorithm for a bootstrap confidence interval is as follows:

- Draw a random sample of size n with replacement from the data (a resample).
- Record the statistic of interest for the resample.
- Repeat steps 1–2 many (R) times.
- For an x% confidence interval, trim [(1 – [x/100]) / 2]% of the R resample results from either end of the distribution.
- The trim points are the endpoints of an x% bootstrap confidence interval


**NOTE:**
- The percentage associated with the confidence interval is termed the level of confidence. 
- The higher the level of confidence, the wider the interval. 
- Also, the smaller the sample, the wider the interval (i.e., the more uncertainty). 
- Both make sense: the more confident you want to be, and the less data you have, the wider you must make the confidence interval to be sufficiently assured of capturing the true value.


**KEY IDEAS:**
- Confidence intervals are the typical way to present estimates as an interval range.
- The more data you have, the less variable a sample estimate will be.
- The lower the level of confidence you can tolerate, the narrower the confidence interval will be.
- The bootstrap is an effective way to construct confidence intervals.
