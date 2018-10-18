## Long-Tailed Distributions:

**Key Ideas :**
- data is generally not normally distributed.
- Assuming a normal distribution can lead to underestimation of extreme events (“black swans”).

- Tail : The long narrow portion of a frequency distribution, where relatively extreme values occur at low frequency.
- Skew : Where one tail of a distribution is longer than the other.

## Student’s t-Distribution:

- The t-distribution is a normally shaped distribution, but a bit thicker and longer on the tails. 
- It is used extensively in depicting distributions of sample statistics. 
- Distributions of sample means are typically shaped like a t-distribution, and there is a family of t-distributions that differ depending on how large the sample is. The larger the sample, the more normally shaped the t-distribution becomes.

**Note**
### What do data scientists need to know about the t-distribution and the central limit theorem? 
Not a whole lot. These distributions are used in classical statistical inference, but are not as central to the purposes of data science. Understanding and quantifying uncertainty and variation are important to data scientists, but empirical bootstrap sampling can answer most questions about sampling error. However, data scientists will routinely encounter t-statistics in output from statistical software and statistical procedures in R, for example in A-B tests and regressions, so familiarity with its purpose is helpful.

**Key Ideas**

- The t-distribution is actually a family of distributions resembling the normal distribution, but with thicker tails.
- It is widely used as a reference basis for the distribution of sample means, differerences between two sample means, regression parameters, and more.

## Binomial Distribution
- Binomial outcomes are important to model, since they represent, among other things, fundamental decisions (buy or don’t buy, click or don’t click, survive or die, etc.).
- A binomial trial is an experiment with two possible outcomes: one with probability p and the other with probability 1 – p.
- With large n, and provided p is not too close to 0 or 1, the binomial distribution can be approximated by the normal distribution.

## Poisson and Related Distributions

Many processes produce events randomly at a given overall rate—visitors arriving at a website, cars arriving at a toll plaza (events spread over time), imperfections in a square meter of fabric, or typos per 100 lines of code (events spread over space).

**Key Ideas**
- For events that occur at a constant rate, the number of events per unit of time or space can be modeled as a Poisson distribution.
- In this scenario, you can also model the time or distance between one event and the next as an exponential distribution.
- A changing event rate over time (e.g., an increasing probability of device failure) can be modeled with the Weibull distribution.
