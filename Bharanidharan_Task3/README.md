# Task 3 – Data Cleaning Using Python

## Overview
This project was completed as part of a **Data Analytics Internship – Task 3**.

The objective is to clean a messy sales dataset using Python, Pandas, and NumPy, identify data quality issues, and prepare the data for further analysis.

## Dataset
- **Dataset Name:** Dirty Sales Data (Dirty Data Sample)
- **Source:** Kaggle
- **Dataset Creator:** Shiva Vashishtha
- **File Format:** Excel (.xlsx)

The dataset contains order IDs, customer segments, shipping modes, and sales values.

## Tools and Technologies
- Python
- Pandas
- NumPy
- Jupyter Notebook

## Data Cleaning Process

### 1. Data Quality Assessment
- Identified missing values and duplicate records.
- Examined column names, data types, and numerical anomalies.
- Generated an initial data quality report.

### 2. Missing Value Handling
- Removed unnecessary header rows and records with missing Order IDs.
- Handled missing sales values based on the structure of the dataset.
- Avoided mean and median imputation to prevent artificial sales values.

### 3. Duplicate Removal
- Checked for duplicate records using `duplicated()`.
- Applied `drop_duplicates()` to ensure data consistency.

### 4. Data Standardization
- Renamed unnamed columns with meaningful names.
- Removed redundant subtotal columns.
- Standardized customer segment and shipping mode column names.

### 5. Outlier Detection
- Applied the Interquartile Range (IQR) method.
- Identified potential outliers in sales values.
- Retained detected outliers because they may represent genuine transactions.

### 6. Data Type Correction
- Converted Order ID to string.
- Converted sales columns to `float64`.

### 7. Before vs. After Comparison
- Compared row counts, missing values, duplicate records, and data types.
- Documented the decisions made during data cleaning.

### 8. Export Cleaned Dataset
- Exported the cleaned dataset as `cleaned_sales_data.csv`.
- Verified the exported CSV using Pandas.

## Project Files

- `Dirty_Data.xlsx` – Original dataset
- `Cleaning Data.ipynb` – Python data cleaning notebook
- `cleaned_sales_data.csv` – Cleaned dataset
- `README.md` – Project documentation

## Key Learnings
- Identifying and handling missing values
- Detecting and removing duplicates
- Standardizing column names and data types
- Detecting outliers using IQR
- Documenting data cleaning decisions
- Exporting cleaned datasets for analysis

## Conclusion
This project demonstrates practical data cleaning techniques using Python. The resulting dataset has a more consistent structure and is better prepared for data analysis and visualization.
