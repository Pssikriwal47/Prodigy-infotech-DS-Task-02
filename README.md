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

## Explanation of the Code:Loading and Inspecting Data:

data=pd.read_csv("test.csv"): Load the CSV file into a DataFrame.data.head(), data.tail(): Preview the first and last 5 rows of the data.
data.describe(): Get a summary of statistics for numerical columns.data.info(): Print the summary of the DataFrame including data types and non-null values.
data.isnull().sum():
Check for missing values in each column.Handling Missing Data:data.
dropna(subset=["Embarked"], inplace=True): Remove rows where the 'Embarked' column has missing values.
data["Cabin"].fillna("Unknown", inplace=True): Replace missing values in the 'Cabin' column with "Unknown".
data["Age"].fillna(data["Age"].mean(), inplace=True): Fill missing 'Age' values with the mean age.
Checking for Duplicates:data.duplicated().sum(): Check if there are any duplicate rows in the data.
Data Visualization:Age Distribution:A histogram and KDE plot to visualize the distribution of 'Age'.
Survival by Gender:A count plot to visualize the distribution of 'Sex' (gender).Age vs.
 Fare Scatter Plot:A scatter plot to explore the relationship between 'Age' and 'Fare', with 'Age' used as the hue for coloring.

```python
import pandas as pd

data = pd.read_csv("test.csv")
data.head()
data.tail()
data.describe()
data.info()
data.isnull().sum()






