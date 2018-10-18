## Normal Distribution:

- Error : The difference between a data point and a predicted or average value.
- Standardize : Subtract the mean and divide by the standard deviation.
- z-score : The result of standardizing an individual data point.
- Standard normal : A normal distribution with mean = 0 and standard deviation = 1.
- QQ-Plot : A plot to visualize how close a sample distribution is to a normal distribution.
- In a normal distribution, 68% of the data lies within one standard deviation of the mean, and 95% lies within two standard deviations.

**NOTE** : Most of the variables used in a typical data science project—in fact most raw data as a whole—are not normally distributed.


## QQ Plot:
- A QQ-Plot is used to visually determine how close a sample is to the normal distribution. 
- The QQ-Plot orders the z-scores from low to high, and plots each value’s z-score on the y-axis; the x-axis is the corresponding quantile of a normal distribution for that value’s rank. 
- If the points roughly fall on the diagonal line, then the sample distribution can be considered close to normal.


**Key Ideas**

- The normal distribution was essential to the historical development of statistics, as it permitted mathematical approximation of uncertainty and variability.
- While raw data is typically not normally distributed, errors often are, as are averages and totals in large samples.
- To convert data to z-scores, you subtract the mean of the data and divide by the standard deviation; you can then compare the data to a normal distribution.
