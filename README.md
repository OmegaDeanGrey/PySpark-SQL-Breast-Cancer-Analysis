# Breast Cancer Analysis with PySpark and Spark SQL

## Overview

This project is part of Course 4, Module 4. It uses PySpark, Spark SQL, Pandas, and Matplotlib to analyze the Breast Cancer Wisconsin Diagnostic dataset.

The lab focuses on data exploration, SQL queries, statistical calculations, and visualization using a distributed data processing framework.

## Dataset

The `breast_cancer.csv` dataset contains 569 patient records with measurements related to breast cancer diagnosis.

Each record is classified as benign (B) or malignant (M).

During preprocessing, an extra empty column (`_c32`) was removed, leaving 32 columns without removing any records.

## Technologies Used

- Python
- PySpark
- Spark SQL
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

## Analysis

The notebook demonstrates how to:

- Create and verify a Spark session.
- Load and inspect CSV data using PySpark.
- Retrieve a specific patient measurement.
- Count benign and malignant diagnoses using PySpark and SQL.
- Visualize diagnosis counts with a bar chart.
- Calculate summary statistics using PySpark functions.
- Compute averages, ratios, and standard deviations using Spark SQL.
- Properly close the Spark session.

## Key Results

| Metric | Result |
|---|---|
| Total records | 569 |
| Benign diagnoses | 357 |
| Malignant diagnoses | 212 |
| Difference (B − M) | 145 |
| 77th record perimeter mean | 87.91 |
| Maximum compactness mean | 0.3454 |
| Minimum smoothness mean | 0.05263 |
| Difference between feature extremes | 0.29277 |
| Product of rounded benign feature averages | 16990.71552 |
| Average malignant radius-to-perimeter ratio | 0.15 |
| Sum of standard deviations | 0.03447464413112017 |

## Running the Project

Install the required Python packages:

```bash
python3 -m pip install pyspark pandas numpy matplotlib pyarrow jupyter
```

A compatible Java installation is also required for PySpark.

Open the supplied Course 4, Module 4 Jupyter notebook in VS Code or Jupyter, ensure `breast_cancer.csv` is in the same directory, and execute the cells in order.

## Notes

The notebook retains the variable name `permiter_mean_value` as written in the supplied CodeGrade instructions, despite the spelling error.

The analysis is exploratory and does not train or evaluate a predictive diagnostic model.