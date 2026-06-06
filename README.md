# Cognify Machine Learning Tasks

This repository contains the solutions for the Cognify data science tasks.

## Task 1: Restaurant Rating Prediction
**Objective:** Build a machine learning model to predict the aggregate rating of a restaurant based on other features.

### Steps Performed
1. **Data Preprocessing:** Handled missing values, encoded categorical variables, and split the data into training and testing sets.
2. **Model Selection & Training:** Selected and trained two regression algorithms: Linear Regression and Decision Tree Regression.
3. **Model Evaluation:** Evaluated the models using Mean Squared Error (MSE) and R-squared ($R^2$) metrics.
4. **Feature Importance Analysis:** Analyzed the most influential features affecting the restaurant ratings.

### Results
Two models were evaluated on the testing data. The Decision Tree Regression model significantly outperformed the Linear Regression model.

| Model | Mean Squared Error (MSE) | R-squared ($R^2$) Score |
|-------|--------------------------|-------------------------|
| Linear Regression | 1.5598 | 0.3147 |
| Decision Tree Regression | 0.1080 | 0.9526 |

Based on the Decision Tree model, the most influential features determining a restaurant's rating are **Votes** (0.9715), **Longitude** (0.0116), **Latitude** (0.0054), **Cuisines** (0.0047), and **Average Cost for two** (0.0030).

---

## Task 2: Restaurant Recommendation
**Objective:** Create a restaurant recommendation system based on user preferences.

### Steps Performed
1. **Data Preprocessing:** Handled missing values (e.g. cuisines) and encoded required variables.
2. **Recommendation Criteria:** Determined the criteria for recommendations based on user's preferred cuisine, price range, and minimum rating.
3. **Content-Based Filtering:** Implemented a TF-IDF vectorizer on restaurant cuisines to compute similarity via cosine similarity against the user's preference.
4. **System Testing:** Created a function to test the recommendation engine against sample user criteria, returning the top matches.

---

## Contents
- `Task1Cognify.ipynb`: Notebook for predicting restaurant ratings.
- `Task2Cognify.ipynb`: Notebook for the content-based restaurant recommendation system.
- `CognifyDataset.csv`: The primary dataset used for the tasks.
