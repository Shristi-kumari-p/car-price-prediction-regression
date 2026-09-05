# car-price-prediction-regression

# 🚗 Car Price Prediction using Regression

## 📌 Project Overview

This project focuses on predicting car prices using **Linear Regression** and **Feature Selection** techniques.

The project follows an end-to-end machine learning workflow, including data understanding, data cleaning, exploratory data analysis (EDA), feature engineering, feature selection, model building, model evaluation, and residual analysis.

The goal is to understand which vehicle characteristics have a significant relationship with car prices and build a regression model capable of predicting the price of a car.

---

## 🎯 Problem Statement

Car prices depend on multiple factors such as the vehicle's make, engine specifications, horsepower, dimensions, fuel type, mileage, and other characteristics.

The objective of this project is to develop a machine learning model that can predict car prices based on these features.

---

## 🎯 Objectives

- Analyze the factors influencing car prices.
- Perform data cleaning and preprocessing.
- Conduct exploratory data analysis to identify important patterns and relationships.
- Apply feature selection to identify relevant predictors.
- Build a Linear Regression model for car price prediction.
- Evaluate model performance using multiple regression metrics.
- Analyze prediction errors using residual analysis.
- Compare model performance before and after feature selection.

---

## 📊 Dataset

The dataset contains **205 records and 26 columns** related to automobile characteristics.

### Target Variable

- `price`

### Important Features

Some of the features used in the analysis include:

- Make
- Fuel Type
- Body Style
- Engine Type
- Engine Size
- Horsepower
- Wheel Base
- Bore
- Stroke
- Compression Ratio
- City MPG
- Highway MPG

---

## 🔍 Exploratory Data Analysis

The following analyses were performed to understand the dataset:

- Target variable distribution
- Numerical feature distributions
- Feature vs. price relationships
- Correlation analysis
- Correlation heatmap
- Outlier analysis
- Identification of important variables affecting car price

### Key EDA Visualizations

#### Price Distribution

![Price Distribution](images/price_distribution.png)

#### Correlation Heatmap

![Correlation Heatmap](images/correlation_heatmap.png)

---

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

- Identified missing values.
- Replaced `"?"` values with missing values.
- Converted relevant columns to appropriate data types.
- Handled missing values.
- Encoded categorical variables.
- Prepared the dataset for machine learning.
- Separated independent variables and the target variable.

---

## 🔧 Feature Selection

Feature selection was performed to identify the variables that have a meaningful relationship with the target variable, `price`.

Features were selected based on their **absolute correlation with the target variable**, using a correlation threshold.

This helped reduce the number of predictors and allowed comparison between the model using the original feature set and the model using selected features.

---

## 🤖 Machine Learning Model

### Linear Regression

Linear Regression was used as the primary machine learning algorithm for predicting car prices.

Two approaches were evaluated:

### Model 1 — Linear Regression with Original Features

The first model was trained using the prepared feature set.

### Model 2 — Linear Regression with Selected Features

The second model was trained using the features selected through the feature selection process.

The performance of both models was compared to understand the impact of feature selection.

---

## 📈 Model Evaluation

The models were evaluated using the following regression metrics:

- **R² Score**
- **Adjusted R²**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **Mean Absolute Percentage Error (MAPE)**

> **Note:** Final model performance reported here should be based on the independent test set rather than training-set results.

### Model Comparison

| Metric | Model 1 | Model 2 |
|---|---:|---:|
| R² | To be updated | To be updated |
| Adjusted R² | To be updated | To be updated |
| MSE | To be updated | To be updated |
| RMSE | To be updated | To be updated |
| MAPE | To be updated | To be updated |

---

## 📊 Actual vs Predicted Prices

The actual vs. predicted plot was used to visually evaluate how closely the model's predictions matched the actual car prices.

![Actual vs Predicted](images/actual_vs_predicted.png)

A prediction closer to the diagonal reference line indicates better agreement between actual and predicted prices.

---

## 📉 Residual Analysis

Residual analysis was performed to understand the errors made by the regression model.

Residuals were analyzed using:

- Residual distribution
- Residual boxplot
- Residual vs. predicted values

![Residual Analysis](images/residual_analysis.png)

Residual analysis helps identify patterns in prediction errors and assess whether the regression model is capturing the underlying relationship appropriately.

---

## 🔎 Key Insights

- Car prices are influenced by multiple vehicle characteristics.
- Engine and performance-related variables show meaningful relationships with price.
- Feature selection helps identify the most relevant predictors.
- Comparing models with original and selected features helps evaluate whether reducing the feature set improves model performance.
- Residual analysis provides additional information about model errors beyond standard evaluation metrics.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy
- Jupyter Notebook

---

## 📁 Project Structure

```text
car-price-prediction-regression/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── notebooks/
│   └── car_price_prediction_regression.ipynb
│
├── data/
│   └── car_price.csv
│
└── images/
    ├── price_distribution.png
    ├── correlation_heatmap.png
    ├── actual_vs_predicted.png
    └── residual_analysis.png
