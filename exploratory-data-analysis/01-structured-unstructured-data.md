## Elements of Structured Data

To apply the statistical concepts, unstructured raw data must be processed and manipulated into a structured form.

### Data types:
There are two basic types of structured data: numeric and categorical. Numeric can be divided in continuous and discrete and Categorical can be divided into - Categorical, Binary and Ordinal.

1. **Continuous** - Data that can take on any value in an interval.
   - Synonyms -interval, float, numeric
2. **Discrete** - Data that can take on only integer values, such as counts.
   - Synonyms - integer, count
3. **Categorical** - Data that can take on only a specific set of values representing a set of possible categories.
   - Synonyms - enums, enumerated, factors, nominal, polychotomous
4. **Binary** - A special case of categorical data with just two categories of values (0/1, true/false).
   - Synonyms - dichotomous, logical, indicator, boolean
5. **Ordinal** - Categorical data that has an explicit ordering.
   - Synonyms - ordered factor


### Why do we bother with a taxonomy of data types? 
- for the purposes of data analysis and predictive modeling, the data type is important to help determine the type of visual display, data analysis, or statistical model.
- Storage and indexing can be optimized (as in a relational database).

### Rectangula Data
- Data frame : Rectangular data (like a spreadsheet) is the basic data structure for statistical and machine learning models.
- Feature : A column in the table is commonly referred to as a feature.
  - Synonyms : attribute, input, predictor, variable
- Outcome : Many data science projects involve predicting an outcome—often a yes/no outcome.
  - Synonyms : dependent variable, response, target, output
- Records : A row in the table is commonly referred to as a record.
  - Synonyms : case, example, instance, observation, pattern, sample

### Non-rectangular data structures:
- time Series
- graph data structures
- spatial data structures
