## Hypothesis Tests:

Hypothesis tests, (also called significance tests) are used to learn whether random chance might be responsible for an observed effect.

**Key Terms:**
1. Null hypothesis : The hypothesis that chance is to blame.
2. Alternative hypothesis : Counterpoint to the null (what you hope to prove).
3. One-way test : Hypothesis test that counts chance results only in one direction.
4. Two-way test : Hypothesis test that counts chance results in two directions.

**NOTE**
- An A/B test is typically constructed with a hypothesis in mind. 
- For example, the hypothesis might be that price B produces higher profit. 

### Why do we need a hypothesis? Why not just look at the outcome of the experiment and go with whichever treatment does better?

The answer lies in the tendency of the human mind to underestimate the scope of natural random behavior. 
- One manifestation of this is the failure to anticipate extreme events, or so-called “black swans”/“Long-Tailed Distributions”. 
- Another manifestation is the tendency to misinterpret random events as having patterns of some significance. Statistical hypothesis testing was invented as a way to protect researchers from being fooled by random chance.

In a properly designed A/B test, you collect data on treatments A and B in such a way that any observed difference between A and B must be due to either:
  - Random chance in assignment of subjects
  - A true difference between A and B

A statistical hypothesis test is analysis of an A/B test, or any randomized experiment, to assess whether random chance is a reasonable explanation for the observed difference between groups A and B.

## Basic philosophy behid hypothesis test?
Hypothesis tests use the following logic: *Given the human tendency to react to unusual but random behavior and interpret it as something meaningful and real, in our experiments we will require proof that the difference between groups is more extreme than what chance might reasonably produce.*


## The Null Hypothesis :
In hypothesis testing we have a baseline assumption that the treatments are equivalent, and any difference between the groups is due to chance. This baseline assumption is termed the **null hypothesis**. 

Our hope is then that we can, in fact, prove the null hypothesis wrong, and show that the outcomes for groups A and B are more different than what chance might produce.

One way to do this is via a resampling permutation procedure, in which we shuffle together the results from groups A and B and then repeatedly deal out the data in groups of similar sizes, then observe how often we get a difference as extreme as the observed difference.

## Alternative Hypothesis :
Hypothesis tests by their nature involve not just a null hypothesis, but also an offsetting alternative hypothesis. Here are some examples:

    Null = “no difference between the means of group A and group B,” alternative = “A is different from B” (could be bigger or smaller)

    Null = “A less-than-or-equal-to B,” alternative = “B > A”

    Null = “B is not X% greater than A,” alternative = “B is X% greater than A”

Taken together, the null and alternative hypotheses must account for all possibilities. The nature of the null hypothesis determines the structure of the hypothesis test.

## One-Way, Two-Way Hypothesis Test:
Often, in an A/B test, you are testing a new option (say B), against an established default option (A) and the presumption is that you will stick with the default option unless the new option proves itself definitively better. 
In such a case, you want a hypothesis test to protect you from being fooled by chance in the direction favoring B. 
You don’t care about being fooled by chance in the other direction, because you would be sticking with A unless B proves definitively better. 
So you want a *directional alternative hypothesis* (B is better than A). In such a case, you use a one-way (or one-tail) hypothesis test. This means that extreme chance results in only one direction direction count toward the p-value.

If you want a hypothesis test to protect you from being fooled by chance in either direction, the alternative hypothesis is bidirectional (A is different from B; could be bigger or smaller). In such a case, you use a two-way (or two-tail) hypothesis. This means that extreme chance results in either direction count toward the p-value.

A one-tail hypothesis test often fits the nature of A/B decision making, in which a decision is required and one option is typically assigned “default” status unless the other proves better.

**Key Ideas**:
- A null hypothesis is a logical construct embodying the notion that nothing special has happened, and any effect you observe is due to random chance.

- The hypothesis test assumes that the null hypothesis is true, creates a “null model” (a probability model), and tests whether the effect you observe is a reasonable outcome of that model.

