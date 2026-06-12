# Car Sales Prediction using Linear Regression

## Project Overview

This project focuses on predicting car sales using Machine Learning and Statistical Modeling techniques.

A car manufacturing company wants to understand which factors influence vehicle sales and use those insights to predict future sales for new car models.

The project uses Linear Regression to identify significant factors affecting sales and build a predictive model capable of estimating future car sales.

---

## Business Problem

A car company wants to launch new vehicle models and maximize sales.

Before introducing a new model, management wants answers to the following questions:

* Which vehicle characteristics increase sales?
* How does price affect sales?
* Does fuel efficiency influence demand?
* Does vehicle type impact sales performance?
* Which manufacturers perform better in the market?
* Can future sales be predicted before launching a vehicle?

To answer these questions, a Linear Regression model was developed.

---

## Dataset Description

The dataset contains historical information about vehicle sales and vehicle characteristics.

### Features Included

* Manufacturer
* Model
* Vehicle Type
* Price
* Engine Size
* Horsepower
* Wheelbase
* Width
* Length
* Fuel Capacity
* Fuel Efficiency
* Latest Launch Date
* Four Year Resale Value
* Sales in Thousands (Target Variable)

### Target Variable

```text
Sales_in_thousands
```

The objective is to predict vehicle sales based on vehicle specifications.

---

## Tools & Technologies Used

### Programming Language

* Python

### Libraries

* NumPy
* Pandas
* Matplotlib
* Seaborn
* SciPy
* Statsmodels
* Scikit-Learn

### Machine Learning Technique

* Multiple Linear Regression

---

## Project Workflow

### 1. Data Understanding

Performed:

* Dataset inspection
* Variable identification
* Data type analysis
* Statistical summary

Methods used:

* info()
* describe()
* shape()
* nunique()

---

### 2. Exploratory Data Analysis (EDA)

Analyzed:

* Distribution of numerical variables
* Correlation between variables
* Missing values
* Outliers

Techniques used:

* Histograms
* Boxplots
* Correlation Matrix
* Scatter Plots

---

### 3. Data Cleaning

Performed:

* Missing value treatment
* Data consistency checks
* Variable transformation

---

### 4. Feature Engineering

Created transformed variables to improve model performance.

### Log Transformation

The target variable was transformed using logarithms to improve:

* Normality
* Model stability
* Error distribution

Example:

```python
new_log_Sales_in_Thousands
```

---

### 5. Train-Test Split

The dataset was divided into:

* Training Dataset
* Testing Dataset

Purpose:

* Train the model on historical data
* Evaluate performance on unseen data

---

## Linear Regression Assumptions Validation

The following assumptions were checked:

### 1. Normality of Residuals

Residuals were analyzed to ensure they approximately followed a normal distribution.

### 2. Linearity

The relationship between predictors and target variable was examined.

### 3. Homoscedasticity

Residual variance was checked to ensure consistency across predictions.

### 4. Independence of Errors

Model residuals were evaluated for independence.

---

## Feature Selection

Feature importance was calculated using:

```python
f_regression()
```

### Objective

Identify variables that significantly influence vehicle sales.

Outputs obtained:

* F Score
* P Value

Features with statistically significant relationships were retained.

---

## Multicollinearity Analysis

Multicollinearity was checked using:

### Variance Inflation Factor (VIF)

Purpose:

* Detect highly correlated independent variables.
* Improve model interpretability.

### VIF Interpretation

| VIF Value | Interpretation            |
| --------- | ------------------------- |
| 1 - 5     | Low Multicollinearity     |
| 5 - 10    | High Multicollinearity    |
| > 10      | Serious Multicollinearity |

Variables with high VIF values were removed iteratively.

---

## Final Model Variables

After feature selection and multicollinearity checks, the final model included:

* Fuel Efficiency
* Price in Thousands
* Wheelbase
* Vehicle Type (Passenger)
* Manufacturer Ford
* Manufacturer Plymouth

These variables showed significant impact on sales prediction.

---

## Model Building

A Multiple Linear Regression model was developed using:

```python
statsmodels.api.OLS
```

The model estimates vehicle sales based on selected features.

---

## Model Evaluation

The model was evaluated using:

### R² Score

Measures the proportion of variation in sales explained by the model.

### Mean Absolute Error (MAE)

Measures average prediction error.

### Mean Squared Error (MSE)

Penalizes larger prediction errors.

### Root Mean Squared Error (RMSE)

Provides error magnitude in the original unit scale.

---

## Key Insights

### Price Impact

Vehicle price significantly influences sales volume.

### Fuel Efficiency

Fuel-efficient vehicles tend to perform better in the market.

### Vehicle Type

Passenger vehicles show distinct sales behavior compared to other vehicle categories.

### Manufacturer Influence

Certain manufacturers demonstrate stronger sales performance.

### Wheelbase Effect

Vehicle dimensions contribute to customer purchasing behavior.

---

## Skills Demonstrated

### Data Analysis

* Exploratory Data Analysis
* Statistical Analysis
* Data Cleaning

### Machine Learning

* Linear Regression
* Feature Selection
* Model Evaluation

### Statistics

* P-Value Interpretation
* Residual Analysis
* Multicollinearity Analysis

### Python

* Pandas
* NumPy
* Scikit-Learn
* Statsmodels
* Data Visualization

---

## Project Structure

```text
Car-Sales-Linear-Regression/
│
├── Car_Sales_Linear_Regression.ipynb
├── Dataset.csv
├── README.md
└── Model Outputs
```

---


## Author

Vishay Gautam

Aspiring Data Analyst
Email:Vishayvee@gmail.com

Skills:

* Python
* SQL
* Excel
* Power BI
* Machine Learning
* Statistical Analysis
