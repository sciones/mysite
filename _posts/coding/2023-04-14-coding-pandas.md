---
title: "Coding: Pandas Tutorial"
date: 2023-04-14
categories:
  - Coding
tags:
  - Coding
  - Pandas
toc: true
toc_label: "Pandas"
toc_icon: "cog"
---

**Introduction to Pandas**: A Beginner's Guide

Pandas is a Python library that provides powerful data manipulation and analysis tools. It's built on top of Numpy, and is an essential tool for data scientists and analysts who work with large and complex datasets.

Pandas provides two primary data structures for working with tabular data: Series and DataFrame. A Series is a one-dimensional array-like object that can hold any data type, while a DataFrame is a two-dimensional table that can hold multiple types of data.

In this guide, we'll cover the basics of working with Pandas, including how to create and manipulate Series and DataFrames, how to filter and select data, and how to perform basic data analysis.

### Installing Pandas

Before we get started with Pandas, we need to install it. If you're using Anaconda, Pandas is likely already installed. If not, you can install it using pip:

    pip install pandas

### Creating a Series

Let's start by creating a simple Series object. We can create a Series by passing a list of values to the Series constructor:

    import pandas as pd

    s = pd.Series([1, 2, 3, 4, 5])
    print(s)

This will output:

    0    1
    1    2
    2    3
    3    4
    4    5
    dtype: int64

By default, Pandas assigns an index to each value in the Series, starting from 0. We can also specify our own index by passing a list of labels to the index parameter:

    s = pd.Series([1, 2, 3, 4, 5], index=['a', 'b', 'c', 'd', 'e'])
    print(s)

This will output:

    a    1
    b    2
    c    3
    d    4
    e    5
    dtype: int64

### Creating a DataFrame

Next, let's create a DataFrame object. We can create a DataFrame by passing a dictionary of lists to the DataFrame constructor:

    data = {'name': ['John', 'Jane', 'Bob', 'Alice'],
            'age': [25, 30, 35, 40],
            'country': ['USA', 'Canada', 'Australia', 'UK']}
    df = pd.DataFrame(data)
    print(df)

This will output:

        name  age    country
    0   John   25        USA
    1   Jane   30     Canada
    2    Bob   35  Australia
    3  Alice   40         UK

By default, Pandas assigns an index to each row in the DataFrame, starting from 0. We can also specify our own index by passing a list of labels to the index parameter:

    data = {'name': ['John', 'Jane', 'Bob', 'Alice'],
            'age': [25, 30, 35, 40],
            'country': ['USA', 'Canada', 'Australia', 'UK']}
    df = pd.DataFrame(data, index=['a', 'b', 'c', 'd'])
    print(df)

This will output:

        name  age    country
    a   John   25        USA
    b   Jane   30     Canada
    c    Bob   35  Australia
    d  Alice   40         UK

### Accessing Data

Now that we have a Series and a DataFrame, let's learn how to access data from them. We can access a single column or multiple columns from a DataFrame by passing the column name(s) to the DataFrame indexing operator:

    # Access a single column
    print(df['name'])

    # Access multiple columns
    print(df[['name', 'age']])

This will output:

    a     John
    b     Jane
    c      Bob
    d    Alice
    Name: name, dtype: object

        name  age
    a   John   25
    b   Jane   30
    c    Bob   35
    d  Alice   40

We can access a single row from a DataFrame using the .loc[] or .iloc[] accessor. The .loc[] accessor takes a label-based index, while the .iloc[] accessor takes a positional index. For example:

    # Access a single row using label-based index
    print(df.loc['a'])

    # Access a single row using positional index
    print(df.iloc[1])

This will output:

    name        John
    age           25
    country      USA
    Name: a, dtype: object

    name        Jane
    age           30
    country    Canada
    Name: b, dtype: object

We can access a single element from a Series using its index:

    s = pd.Series([1, 2, 3, 4], index=['a', 'b', 'c', 'd'])
    # access a single element from the Series using its index label
    print(s['c'])

This will output:

    3

### Filtering Data

Pandas makes it easy to filter data based on specific conditions. We can use the comparison operators (<, >, ==, etc.) to create boolean masks, and then pass those masks to the DataFrame indexing operator to select the rows that meet the condition. For example:

    # Filter rows where age is greater than 30
    print(df[df['age'] > 30])

    # Filter rows where country is not USA
    print(df[df['country'] != 'USA'])

This will output:

        name  age    country
    c    Bob   35  Australia
    d  Alice   40         UK

        name  age    country
    b   Jane   30     Canada
    c    Bob   35  Australia
    d  Alice   40         UK

### Data Analysis

Pandas also provides a range of tools for basic data analysis. For example, we can use the `.describe()` method to get summary statistics for a DataFrame:

    print(df.describe())

This will output:

                age
    count   4.000000
    mean   32.500000
    std     7.905694
    min    25.000000
    25%    28.750000
    50%    32.500000
    75%    36.250000
    max    40.000000

We can also use the `.groupby()` method to group rows by a specific column and perform aggregations:

    # Group by country and calculate mean age
    print(df.groupby('country')['age'].mean())

This will output:

    country
    Australia    35
    Canada       30
    UK           40
    USA          25
    Name: age, dtype: int64

### Conclusion

In this guide, we covered the basics of working with Pandas, including how to create and manipulate Series and DataFrames, how to filter and select data, and how to perform basic data analysis. Pandas is a powerful tool for data manipulation and analysis, and is essential for any data scientist or analyst who works with large and complex datasets.