# Data-Cleaning-Pipeline

This repository provides a robust and reusable data cleaning pipeline implemented in Python using the pandas library. The `data_cleaning_pipeline.py` script automates several essential data preprocessing steps, ensuring data quality and consistency for machine learning or data analysis.

## Purpose

The primary purpose of this pipeline is to streamline the data cleaning process, which is a crucial step in any data science project. By automating these tasks, this script helps to:

* Reduce manual effort and save time.
* Improve the accuracy and reliability of data analysis.
* Ensure that data is in a suitable format for modeling.

## Features

The pipeline encompasses the following key features:

1.  **Missing Value Handling:**
    * Categorical features: Missing values are imputed with the mode (most frequent value) to preserve the distribution of categorical data.
    * Numerical features: Missing values are imputed with the median, which is robust to outliers.

2.  **Outlier Handling:**
    * Outliers in numerical features are identified and removed using the IQR method. This helps to mitigate the impact of extreme values on subsequent analysis.

3.  **Feature Scaling:**
    * Numerical features are standardized using the StandardScaler. This ensures that all features have a mean of 0 and a standard deviation of 1, which is often necessary for many machine learning algorithms.
