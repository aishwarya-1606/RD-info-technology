# 📊 Task 1: Data Collection and Cleaning

## Overview
This project focuses on collecting raw data and performing data cleaning to ensure the dataset is accurate, consistent, and ready for analysis. Data preprocessing is an essential step in the data science workflow as it improves data quality and helps generate reliable insights.

## Objectives
- Collect data from various sources.
- Identify and handle missing values.
- Remove duplicate records.
- Correct inconsistent or invalid data.
- Prepare the dataset for further analysis and machine learning tasks.

## Tools Used
- Python
- Pandas
- NumPy
- Jupyter Notebook

## Steps Performed

### 1. Data Collection
- Imported data from CSV/Excel files.
- Loaded the dataset into a Pandas DataFrame.

### 2. Data Inspection
- Examined dataset structure and data types.
- Checked for missing values and duplicate records.

### 3. Data Cleaning
- Removed or filled missing values.
- Eliminated duplicate entries.
- Standardized data formats where necessary.
- Verified data consistency.

### 4. Data Preparation
- Created a clean dataset suitable for analysis and visualization.

## Sample Code

```python
import pandas as pd

# Load dataset
df = pd.read_csv("data.csv")

# Check missing values
df.isnull().sum()

# Fill missing values
df.fillna(method='ffill', inplace=True)

# Remove duplicates
df.drop_duplicates(inplace=True)

# Dataset information
df.info()
