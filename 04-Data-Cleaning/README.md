# Data Cleaning

Data come in many formats and vary greatly in usefulness for analysis. Although we would prefer all our data to come in a tabular format with each value recorded consistently and accurately, in reality we must carefully check our data for potential issues that can eventually result in incorrect conclusions.

The term "**data cleaning**" refers to the process of combing through the data and deciding how to resolve inconsistencies and missing values. We will discuss common problems found in datasets and approaches to address them.

## Data cleaning has inherent limitations. 
For example, no amount of data cleaning will fix a biased sampling process. Before embarking on the sometimes lengthy process of data cleaning, we must be confident that our data are collected accurately and with as little bias as possible. Only then can we investigate the data itself and use data cleaning to resolve issues in the data format or entry process.


## Understanding the Data Generation¶

You should ask some questions to the data beforestarting with data cleaning or processing. 

These questions are related to how the data were generated, so data cleaning will usually not be able to resolve issues that arise here.

### What do the data contain? 
This will help you get a bigger picture about the data. Who gave you data? Format of data? What is it consist of? Features variables? etc.

### Are the data a census? 
This depends on our population of interest. For example, if we are interested in calls for service within the last 180 days for crime incidents then the Calls dataset is a census. However, if we are interested in calls for service within the last 10 years the dataset is clearly not a census.

### If the data form a sample, is it a probability sample? 
If we are investigating a period of time that the data do not have entries for, the data do not form a probability sample since there is no randomness involved in the data collection process — we have all data for certain time periods but no data for others.

### What limitations will this data have on our conclusions? 
Although we will ask this question at each step of our data processing, we can already see that our data impose important limitations. The most important limitation is that we cannot make unbiased estimations for time periods not covered by our datasets.

