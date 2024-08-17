# Prodigy InfoTech Data Science Internship Task 2:
<br>
<img src="![ds 02](https://github.com/user-attachments/assets/c5c5b578-a703-4955-a92c-f2d8daa917d7)

"

# Titanic Data Analysis

This repository contains code that performs basic data analysis and visualization on the Titanic dataset. The code handles data preprocessing, deals with missing values, and visualizes key relationships within the data.

## Table of Contents
- [Introduction](#introduction)
- [Data Loading and Initial Inspection](#data-loading-and-initial-inspection)
- [Data Preprocessing](#data-preprocessing)
  - [Handling Missing Values](#handling-missing-values)
  - [Checking for Duplicates](#checking-for-duplicates)
- [Data Visualization](#data-visualization)
  - [Age Distribution](#age-distribution)
  - [Survival by Gender](#survival-by-gender)
  - [Age vs. Fare Scatter Plot](#age-vs-fare-scatter-plot)

## Introduction

The code in this repository is designed to work with the Titanic dataset. It performs basic preprocessing and visualizations to understand the distribution of age, gender, and fare among the passengers. This analysis is useful for identifying trends and patterns that could inform more detailed studies or machine learning models.

## Data Loading and Initial Inspection

The dataset is loaded using the pandas library, and the initial inspection involves:

- Previewing the first and last five rows of the dataset.
- Descriptive statistics for numerical columns.
- Summary information about the dataset, including data types and non-null counts.
- Checking for missing values in each column.

```python
import pandas as pd

data = pd.read_csv("test.csv")
data.head()
data.tail()
data.describe()
data.info()
data.isnull().sum()






