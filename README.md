# Linear Regression using only Pandas and NumPy
## Overview
In real-world scenarios, we often face constraints like limited time, resources, and tools. However, the work must get done. This project embraces that mindset. By relying solely on two essential libraries (Pandas and NumPy) I solved the classic machine learning problem: Linear Regression.
The goal was to explore how problems can be solved effectively even with limited tools. Instead of advanced machine learning libraries like Scikit-learn, the project builds everything step by step — including data preprocessing, manual calculations, model training, and evaluation metrics.
This approach demonstrates the power of fundamental concepts while enhancing Python coding skills, algorithmic thinking, and a deeper understanding of the mathematical foundation of linear regression and machine learning techniques.

## Python version: 3.7.4
## Packages used
* numpy
* pandas

## Key Highlights
* Checked for missing values
* Split into train and test
* Remove irrelevant features
* Determine he intercept and coefficients
* Check MSE and MAE

## Dataset
'load_diabetes' data from sklearn.datasets is used for the project. Dataset has:
* 10 numerical features
* one numerical target variable
* 442 observations

## Data Preprocessing and Cleaning
* Used isnull() to check for missing values, and no missing values were found in the dataset.

* Determined the correlation between features and the target variable using Pearson correlation, and removed two (sex and s2)features with correlation values between -0.2 and 0.2. 

* In addition, Pearson correlation was used to examine the linear relationships between features. No features were removed in this step, as the absolute correlation between any two features did not exceed 0.8.


<pre> β = (XᵀX)⁻¹ Xᵀy </pre>

