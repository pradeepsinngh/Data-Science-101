## Estimates of Location

Variables with measured or count data might have thousands of distinct values. A basic step in exploring your data is getting 
a “typical value” for each feature (variable): an estimate of where most of the data is located (i.e., its central tendency).

- Mean : The sum of all values divided by the number of values.
  - Synonyms : average
- Weighted mean : The sum of all values times a weight divided by the sum of the weights.
  - Synonyms : weighted average
- Median : The value such that one-half of the data lies above and below.
  - Synonyms : 50th percentile
- Weighted median : The value such that one-half of the sum of the weights lies above and below the sorted data.
- Trimmed mean : The average of all values after dropping a fixed number of extreme values.
  - Synonyms : truncated mean
- Robust : Not sensitive to extreme values.
  - Synonyms : resistant
- Outlier : A data value that is very different from most of the data.
  - Synonyms : extreme value


**NOTE:** While the mean is easy to compute, it may not always be the best measure for a central value. For this reason, statisticians have developed several alternative estimates to the mean.

## Metrics and Estimates:
statisticians estimate, and data scientists measure.

Statisticians often use the term estimates for values calculated from the data at hand, to draw a distinction between what we see from the data, and the theoretical true or exact state of affairs. 

Data scientists are more likely to refer to such values as a metric. 

The difference reflects the approach of statistics versus data science: accounting for uncertainty lies at the heart of the discipline of statistics, whereas concrete business or organizational objectives are the focus of data science.

## Why use trimmed and weighted mean?

### Trimmed Mean:
- A trimmed mean eliminates the influence of extreme values.
- Eg: In international diving the top and bottom scores from five judges are dropped, and the final score is the average of the three remaining judges. This makes it difficult for a single judge to manipulate the score, perhaps to favor his country’s contestant. 
- Trimmed means are widely used, and in many cases, are preferable to use instead of the ordinary mean

### Weighted Mean: 
there are 2 main reasons -- 
- weighted mean is robust to outliers.
- Some values are intrinsically more variable than others, and highly variable observations are given a lower weight. For example, if we are taking the average from multiple sensors and one of the sensors is less accurate, then we might downweight the data from that sensor.
- The data collected does not equally represent the different groups that we are interested in measuring. For example, because of the way an online experiment was conducted, we may not have a set of data that accurately reflects all groups in the user base. To correct that, we can give a higher weight to the values from the groups that were underrepresented.

### Median and Robust Estimates:

- The median is referred to as a robust estimate of location since it is not influenced by outliers (extreme cases) that could skew the results. 

**NOTE:** When outliers are the result of bad data, the mean will result in a poor estimate of location, while the median will be still be valid.

### Trimmed Mean VS Median: What to use?
The median is not the only robust estimate of location. In fact, a trimmed mean is widely used to avoid the influence of outliers. For example, trimming the bottom and top 10% (a common choice) of the data will provide protection against outliers in all but the smallest data sets. The trimmed mean can be thought of as a compromise between the median and the mean: it is robust to extreme values in the data, but uses more data to calculate the estimate for location.


### Key Ideas:
1. The basic metric for location is the mean, but it can be sensitive to extreme values (outlier).
2. Other metrics (median, trimmed mean) are more robust.

