## Random Sampling and Sample Bias --

1. Sample - A subset from a larger data set.
2. Population - The larger data set or idea of a data set.
3. N (n) - The size of the population (sample).
4. Random sampling - Drawing elements into a sample at random.
5. Stratified sampling - Dividing the population into strata and randomly sampling from each strata.
6. Simple random sample - The sample that results from random sampling without stratifying the population.
7. Sample bias - A sample that misrepresents the population.


**Random Sampling** 
- is a process in which each available member of the population being sampled has an equal chance of being chosen for the sample at each draw. 
- The sample that results is called a simple random sample. 
- Sampling can be done with/ without replacement.

**Data quality** often matters more than data quantity when making an estimate or a model based on a sample. 
- Data quality in data science involves completeness, consistency of format, cleanliness, and accuracy of individual data points. Statistics adds the notion of representativeness.

**Sample Bias** is a bias in which a sample is collected in such a way that some members of the intended population are less likely to be included than others.


### Self-Selection Sampling Bias

The reviews of restaurants, hotels, cafes, and so on that you read on social media sites like Yelp are prone to bias because the people submitting them are not randomly selected; rather, they themselves have taken the initiative to write. This leads to **self-selection bias** - the people motivated to write reviews may be those who had poor experiences, may have an association with the establishment, or may simply be a different type of person from those who do not write reviews.

### Bias
- refers to measurement or sampling errors that are produced by the measurement or sampling process. 
- An important distinction should be made between errors due to random chance, and errors due to bias. 
- Consider the physical process of a gun shooting at a target. It will not hit the absolute center of the target every time, or even much at all. An unbiased process will produce error, but it is random and does not tend strongly in any direction (see Figure 2-2). The results will show a biased process—there is still random error in both the x and y direction, but there is also a bias. Shots tend to fall in the upper-right quadrant.

## Random Selection
### How to solve the problem of sample bias? 
Ans : Use Random Sampling.

In **stratified sampling**, the population is divided up into strata, and random samples are taken from each stratum. 


### Size versus Quality: When Does Size Matter?
- In the era of big data, it is sometimes surprising that smaller is better. 
- Time and effort spent on random sampling not only reduce bias, but also allow greater attention to data exploration and data quality. 
- For eg, missing data and outliers may contain useful information. It might be prohibitively expensive to track down missing values or evaluate outliers in millions of records, but doing so in a sample of several thousand records may be feasible. Data plotting and manual inspection bog down if there is too much data.

### So when are massive amounts of data needed?
- The classic scenario for the value of big data is when the data is not only big, but sparse as well.


### Sample Mean versus Population Mean: Why make the distinction? 
Information about samples is observed, and information about large populations is often inferred from smaller samples.

## Key Ideas:
1. Even in the era of big data, random sampling remains an important arrow in the data scientist’s quiver.

2. Bias occurs when measurements or observations are systematically in error because they are not representative of the full population.

3. Data quality is often more important than data quantity, and random sampling can reduce bias and facilitate quality improvement that would be prohibitively expensive.
