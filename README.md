# Cognify Task 1: Restaurant Rating Prediction

This repository contains the solution for Cognify Task 1.

## Objective
Build a machine learning model to predict the aggregate rating of a restaurant based on other features.

## Steps Performed
1. **Data Preprocessing:** Handled missing values, encoded categorical variables, and split the data into training and testing sets.
2. **Model Selection & Training:** Selected and trained two regression algorithms: Linear Regression and Decision Tree Regression.
3. **Model Evaluation:** Evaluated the models using Mean Squared Error (MSE) and R-squared ($R^2$) metrics.
4. **Feature Importance Analysis:** Analyzed the most influential features affecting the restaurant ratings.

## Results

### Model Performance
Two models were evaluated on the testing data. The Decision Tree Regression model significantly outperformed the Linear Regression model.

| Model | Mean Squared Error (MSE) | R-squared ($R^2$) Score |
|-------|--------------------------|-------------------------|
| Linear Regression | 1.5598 | 0.3147 |
| Decision Tree Regression | 0.1080 | 0.9526 |

### Top Influential Features
Based on the Decision Tree model, the most influential features determining a restaurant's rating are:
1. **Votes:** 0.9715 (Most dominant feature)
2. **Longitude:** 0.0116
3. **Latitude:** 0.0054
4. **Cuisines:** 0.0047
5. **Average Cost for two:** 0.0030

## Contents
- `Task1Cognify.ipynb`: Jupyter Notebook containing the complete task implementation, data preprocessing, model training, and evaluation.
