Project Overview
The dataset used in this project, melb_data.csv, contains real estate information, while Drugs_product.csv provides details on pharmaceutical products. We cleaned and preprocessed these datasets to prepare them for analysis.

Key Steps
Loading Data and Initial Exploration

Loaded datasets using pandas.
Used Data.info() and Data.isnull().sum() to examine null values and data types.
Visualizing Missing Data

Visualized missing data using seaborn heatmaps to identify patterns.
Handling Missing Values

Mean and Median Imputation: Replaced missing values in numerical columns (Car and BuildingArea) with mean and median values.
Forward and Backward Fill: Filled missing values in YearBuilt and CouncilArea columns with forward and backward fill techniques.
Outlier Treatment

Checked for outliers in the BuildingArea column using describe() and treated them by replacing missing values with the median.
Statistical Analysis

Used the Shapiro-Wilk Test to check if the Car column data follows a normal distribution.
Random Sample Imputation Function

Created a custom function random_sample_imputation to fill missing values by sampling existing non-null values in each column.
Interpolation

Interpolated missing dates in Drugs_product.csv to maintain a logical sequence for time-series data.
Dependencies
Python libraries: pandas, numpy, seaborn, matplotlib, and scipy.
Install all libraries using:

bash
Copy code
pip install pandas numpy seaborn matplotlib scipy
How to Run the Project
Clone this repository.
Run data_cleaning.ipynb or data_cleaning.py to execute the data preprocessing steps.
Use df_imputed as the final cleaned dataset for further analysis.
Results
After completing the data cleaning and preprocessing steps, the datasets are free of missing values, ready for statistical analysis, and optimized for model training.

