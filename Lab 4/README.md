# Lab 4 - Data Quality Assessment & Preprocessing

This notebook applies preprocessing techniques on the Dirty Cafe Sales dataset 
which contains 10,000 cafe transactions with missing values and inconsistent entries.

## Dataset
- **File:** dirty_cafe_sales.csv
- **Rows:** 10,000 | **Columns:** 8

## Tasks results

- **Task 1:** Identified data quality issues including missing values, ERROR/UNKNOWN 
  entries, and wrong data types
- **Task 2:** Checked data types, missing counts, and duplicates
- **Task 3:** Used median imputation for numerical columns and mode for categorical ones
- **Task 4:** Detected and removed 250 outliers in Total Spent using IQR method
- **Task 5:** Applied Min-Max and Z-Score normalization on numerical features
- **Task 6:** Checked correlation between features before applying PCA
- **Task 7:** Applied PCA and reduced 3 features to 2 components keeping 96.6% of variance
