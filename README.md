Heart Attack Risk Prediction

This project analyzes a dataset of patient health metrics to predict the risk of a heart attack. It performs comprehensive Exploratory Data Analysis (EDA), handles class imbalance using SMOTE, and evaluates multiple Machine Learning models to identify at-risk patients.

📊 Project Overview

Goal: Predict binary Heart Attack Risk (1 = Risk, 0 = No Risk).

Data Cleaning: Handled missing values, split blood pressure into systolic/diastolic, encoded categorical variables, and removed irrelevant geographic features.

Class Imbalance: Addressed the 2:1 imbalance (more healthy patients than sick ones) using SMOTE (Synthetic Minority Over-sampling Technique) and Class Weights.

🛠️ Models Evaluated

The following algorithms were implemented and compared:

Logistic Regression: Baseline model (with balanced class weights).

Random Forest Classifier: Ensemble method to handle non-linear relationships.

Decision Tree: Interpretable rule-based model.

k-Nearest Neighbors (k-NN): Distance-based classification.


📈 Key Findings

Geographic Independence: Analysis showed that patient location (Country/Continent) had no significant impact on heart attack risk.

Imbalance Impact: Initial models achieved high accuracy but low recall (missing sick patients). Balancing the data using SMOTE/Class Weights significantly improved the identification of at-risk patients.

