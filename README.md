# SWYNEX Task 1: Data Cleaning & Preparation

## Dataset
Titanic passenger dataset (loaded from the Seaborn library, originally from Kaggle).
The raw dataset had 891 rows and 15 columns.

## Problems Found
- Missing values: age (177), embarked (2), embark_town (2), deck (688)
- 107 duplicate rows
- Inconsistent text formatting in text columns
- Incorrect data types (age stored as decimal, survived as text/boolean)

## What I Did
1. Removed 107 duplicate rows
2. Filled missing age values with the median age
3. Filled missing embarked and embark_town values with the most common value
4. Dropped the deck column because most of its values were missing
5. Cleaned text columns (converted to lowercase and removed extra spaces)
6. Converted columns to the correct data types

## Result
- Rows before cleaning: 891
- Rows after cleaning: 784
- Missing values after cleaning: 0

## Tools Used
Python, Pandas, Google Colab

## Files
- original_titanic (1).csv: raw dataset
- cleaned_titanic (1).csv: cleaned dataset
- Untitled0.ipynb: full Python code used for cleaning
