## Structure:

The structure of a dataset refers to the "shape" of the data files. At a basic level, this refers to the format that the data are entered in.

Here is a list of the most common formats:

- Comma-Separated Values (CSV) and Tab-Separated Values (TSV): These files contain tabular data delimited by either a comma for CSV or a tab character (\t) for TSV. These files are typically easy to work with because the data are entered in a similar format to DataFrames.

- JavaScript Object Notation (JSON): These files contain data in a nested dictionary format. Typically we have to read in the entire file as a Python dict and then figure out how to extract fields for a DataFrame from the dict.

- eXtensible Markup Language (XML) or HyperText Markup Language (HTML): These files also contain data in a nested format.

- Log data: Many applications will output some data as they run in an unstructured text format.


## Structure Checklist

You should have answers to the following questions after looking at the structure of your datasets. 

1. Are the data in a standard format or encoding?
Standard formats include:
```
Tabular data: CSV, TSV, Excel, SQL
Nested data: JSON, XML
```

2. Are the data organized in records (e.g. rows)? If not, can we define records by parsing the data?
3. Are the data nested? If so, can we reasonably unnest the data?
4. Do the data reference other data? If so, can we join the data?
5. What are the fields (e.g. columns) in each record? What is the type of each column?
