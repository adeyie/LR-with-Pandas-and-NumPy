# Linear Regression (LR) using only Pandas and NumPy
## Overview
In real-world scenarios, we often face constraints like limited time, resources, and tools. However, the work must get done. This project embraces that mindset. By relying solely on two essential libraries (Pandas and NumPy) I solved the classic machine learning problem: Linear Regression (LR).
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
  
### All steps from this point forward are based on the training data and applied to test data also, while evaluation metrics are determined using the test data.
  
* The dataset was split into training and testing sets, with 80% of the data used for training and the remaining 20% for testing.
  
* Determined the correlation between features and the target variable using Pearson correlation, and removed two (sex and s2)features with correlation values between -0.2 and 0.2. 

* In addition, Pearson correlation was used to examine the linear relationships between features. No features were removed in this step, as the absolute correlation between any two features did not exceed 0.8.

* The dataset was scaled to the range [0,1], rescaling each feature by subtracting the minimum value and dividing by the range (maximum - minimum) to ensure uniformity across features.

## Model Training
The intercept and coefficients of the LR model were determined using the following matrix form equation.
<pre> β = (XᵀX)⁻¹ Xᵀy </pre>

where,

X: Feature matrix of shape (𝑛,𝑚+1) [with a column of ones for intercept] 

n: number of observations in train data

m: number of features

y: Target vector of shape (n,1)

β: Parameter vector (coefficients) of shape (m+1,1)

After estimating β, the target variable y using the below equation:
<pre> y = Xβ </pre>

## Evaluation Metrics
The evaluation metrics, Mean Squared Error (MSE) and Mean Absolute Error (MAE), were determined for the test data. 

## Concluding Remarks
In conclusion, this project demonstrated solving a linear regression problem using only Pandas and NumPy. By applying fundamental machine learning concepts, I gained insights into data preprocessing, model training, and evaluation, reinforcing key programming and statistical principles.
