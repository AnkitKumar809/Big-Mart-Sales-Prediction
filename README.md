# BigMart Sales Prediction

This project aims to predict the sales of products at different BigMart outlets using various machine learning techniques. The dataset consists of historical sales data for different products across multiple outlets.

## Introduction

The goal of this project is to develop a machine learning model to predict the sales of items in various BigMart outlets. This can help the company in optimizing its inventory management and improving sales strategies.

## Dataset

The dataset contains sales data for 1559 products across 10 stores over a period of 2 years. It includes the following files:
- `train.csv`: Training data
- `test.csv`: Test data

## Exploratory Data Analysis

We perform EDA to understand the dataset better. This involves visualizing the data, checking for missing values, and understanding the distribution of various features.

## Data Preprocessing

We handle missing values and perform label encoding for categorical variables. Standard scaling is applied to the numerical features to ensure the models perform better.

### Handling Missing Values

- `Item_Weight`: Filled with mean values
- `Outlet_Size`: Filled with mode values

### Encoding Categorical Variables

We use `LabelEncoder` to convert categorical features into numerical values.

### Feature Selection

We drop the `Item_Identifier` and `Outlet_Identifier` columns as they are not required for model training.

## Model Building

We build and train multiple models including:
- Linear Regression
- Random Forest Regressor

## Model Evaluation

We evaluate the models using metrics such as:
- R-squared
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

## Hyperparameter Tuning

We use `GridSearchCV` to perform hyperparameter tuning for the Random Forest Regressor to improve its performance.

