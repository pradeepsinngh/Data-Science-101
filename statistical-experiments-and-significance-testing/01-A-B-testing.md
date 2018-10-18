## A/B Testing:

- An A/B test is an experiment with two groups to establish which of two treatments, products, procedures, or the like is superior. 
- Often one of the two treatments is the standard existing treatment, or no treatment. If a standard (or no) treatment is used, 
it is called the control. 
- A typical hypothesis is that treatment is better than control.

**Key Terms**:
- Treatment: Something (drug, price, web headline) to which a subject is exposed.
- Treatment group: A group of subjects exposed to a specific treatment.
- Control group: A group of subjects exposed to no (or standard) treatment.
- Randomization: The process of randomly assigning subjects to treatments.
- Subjects: The items (web visitors, patients, etc.) that are exposed to treatments.
- Test statistic: The metric used to measure the effect of the treatment.

### A/B Testing
A proper A/B test has subjects that can be assigned to one treatment or another. The subject might be a person, a plant seed, a web visitor; the key is that the subject is exposed to the treatment. Ideally, subjects are randomized (assigned randomly) to treatments. In this way, you know that any difference between the treatment groups is due to one of two things:

1. The effect of the different treatments
2. Luck of the draw in which subjects are assigned to which treatments (i.e., the random assignment may have resulted in the naturally better-performing subjects being concentrated in A or B)

### Test Statistics
- the test statistic or metric is used to compare group A to group B. 
- Perhaps the most common metric in data science is a binary variable: click or no-click, buy or don’t buy, fraud or no fraud, and so on.

### Why Have a Control Group?
Why not skip the control group and just run an experiment applying the treatment of interest to only one group, and compare the outcome to prior experience?

Without a control group, there is no assurance that “other things are equal” and that any difference is really due to the treatment (or to chance). When you have a control group, it is subject to the same conditions (except for the treatment of interest) as the treatment group. If you simply make a comparison to “baseline” or prior experience, other factors, besides the treatment, might differ.

**NOTE** 
- In a standard A/B experiment, you need to decide on one metric ahead of time. 
 - Selecting a test statistic after the experiment is conducted opens the door to researcher bias.
 
### Why Just A/B? Why Not C, D…?
Additional treatments can be included.


**Key Ideas**:
- Subjects are assigned to two (or more) groups that are treated exactly alike, except that the treatment under study differs from one to another.

- Ideally, subjects are assigned randomly to the groups.
