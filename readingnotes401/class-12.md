# Pandas

## What is Pandas?

Pandas is a Dataframe to store large quantities of data. NumPy arrays have one dtype versus pandas DataFrame have one dtype per column.
Accessing and processing data in pandas is below:

```python
DataFrame.head() - to access the top of the dataframe.
DafaFrame.tail() - to access the bottom rows of the dataframe.
DataFrame.index or DataFrame.columns will give you access to view data in the dataframe.
DataFrame.to_numpy() - gives the NUmPy representation of the data. 
describe() - shows the quick statistic summary of the data.
DataFrame.sort_index() - sorts by axis.
DataFrame.sort_values() - sorts by values.
DataFrame.at(), DataFrame.iat(), DataFrame.loc(), DataFrame.iloc() - are all ways to select, pinpoint, and locate specific data.
DataFrame.dropna() - drops rows with missing data.
DataFrame.fillna() - fills missing data.
isna() - gets the boolean mask where the values are nan(not a number).
DataFrame.apply() applies a user defined functionto the data.
concat() - method to concatenate pandas objects together along an axis. 
merge() enables SQL style join types along a specific axis.
sum() - 
```

## Things I want to know more about

## Resources

[10 minutes to pandas](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)

[What is Pandas? Why and How to Use Pandas in Python](https://www.youtube.com/watch?v=dcqPhpY7tWk&t=391s)

- >[Advanced Software Development](README.md)
