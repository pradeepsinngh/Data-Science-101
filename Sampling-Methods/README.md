# Sampling Methods

In the age of Big Data, we are tempted to deal with bias by collecting more data. After all, we know that a census will give us perfect estimates; shouldn't a very large sample give almost perfect estimates regardless of the sampling technique?

## Why Probability Sampling

Probability sampling enables us to quantify our uncertainty about an estimation or prediction. 

It is only through this precision that we can conduct inference and hypothesis testing. Be wary when anyone gives you p-values or confidence levels without a proper explanation of their sampling techniques.

Unlike convenience sampling, probability sampling allows us to assign a precise probability to the event that we draw a particular sample.

### Simple Random Sample (SRS):

Suppose we have a population of 6 individuals. We've given each individual a different letter from A−F.
To take an simple random sample of size 2 from this population, we can write each letter A−F on a single index card, place all the cards into a hat, mix the cards well, and draw 2 cards without looking. That is, a SRS is sampling uniformly at random without replacement.

Here are all possible samples of size 2: AB, AC, AD, AE, AF, BC, BD, BE, BF, CD, CE, CF, DE, DF, EF.

There are 15 possible samples of size 2 from our population of 6. Another way to count the number of possible samples is:
```
(6C2) = 6!/ 2!4!=15
```

Since in a SRS we sample uniformly at random, each of these 15 samples are equally likely to be chosen: 
```
P(AB)= P(CD)= …= P(DF)= 1/15
```

We can also use this chance mechanism to answer other questions about the composition of the sample. For example:
```
P(A in sample)= 5/15= 1/3
```
Since 5 out of 15 of the possible samples listed above contain A.

### Two alternative methods of probability sampling: Cluster sampling and Stratified sampling

## Cluster sampling:
In cluster sampling, we divide the population into clusters. Then, we use SRS to select clusters at random instead of individuals.

As an example, suppose we take our population of 6 individuals and we pair each of them up: (A,B)(C,D)(E,F) to form 3 clusters of 2 individuals. Then, we use SRS to select one cluster to produce a sample of size 2.

As before, we can compute the probability that A is in our sample:
```
P(A in sample)= P(AB drawn)= 1/3
```
Similarly the probability that any particular person appears in our sample is 1/3. Note that this is the same as our SRS. 

However, we see differences when we look at the samples themselves. For example, in a SRS the chance of getting AB is the same as the chance of getting AC: 1/15. However, with this cluster sampling scheme:
```
P(AB)= 1/3
P(AC)= 0
```
Since A and C can never appear in the same sample if we only select one cluster.

Cluster sampling is still probability sampling since we can assign a probability to each potential sample. However, the resulting probabilities are different than using a SRS depending on how the population is clustered.

### Why use cluster sampling? 
Cluster sampling is most useful because it makes sample collection easier. For example, it is much easier to poll towns of 100 people each than to poll thousands of people distributed across the entire US. This is the reason why many polling agencies today use forms of cluster sampling to conduct surveys.

The main **downside of cluster sampling** is that it tends to produce greater variation in estimation. This typically means that we take larger samples when using cluster sampling.


## Stratified sampling
In stratified sampling, we divide the population into strata, and then produce one simple random sample per strata. In both cluster sampling and stratified sampling we split the population into groups; in cluster sampling we use a single SRS to select groups whereas in stratified sampling we use multiple SRS's, one for each group.


We can divide our population of 6 individuals into the following strata:
```
Strata 1: {A,B,C,D}
Strata 2: {E,F}
```
We use an SRS to select one individual from each strata to produce a sample of size 2. This gives us the following possible samples:
```
(A,E) (A,F) (B,E) (B,F) (C,E) (C,F) (D,E) (D,F)
```
Again, we can compute the probability that A is in our sample:
```
P(A in sample)= P(A selected from Strata 1)= 1/4
```
However: ```P(AB)=0``` since A and B cannot appear in the same sample.

As you may have figured out, stratified sampling can perhaps be called the proper way to conduct quota sampling. It allows the researcher to ensure that subgroups of the population are well-represented in the sample without using human judgement to select the individuals in the sample. This can often result in less variation in estimation. 

However, stratified sampling is sometimes more difficult to accomplish because we sometimes don't know how large each strata is.



# Takeaways

Before accepting the results of a data analysis, it pays to carefully inspect the quality of the data. In particular, we must ask the following questions:
- Is the data a census (does it include the entire population of interest)?
- If the data is a sample, how was the sample collected? To properly conduct inference, the sample should have been collected according to a completely described probability sampling method.
- What changes were made to the data before producing results? Do any of these changes affect the quality of the data?

