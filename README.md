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

🚀 Installation & Usage

Clone the repository:

git clone [https://github.com/YOUR_USERNAME/heart-attack-prediction.git](https://github.com/YOUR_USERNAME/heart-attack-prediction.git)
cd heart-attack-prediction


Install dependencies:

pip install -r requirements.txt


Run the Analysis:

Step 1: Data Cleaning & EDA:
Run eda_heart_analysis.py to clean the raw data and generate the balanced dataset.

python eda_heart_analysis.py


Step 2: Train Models:
Run any of the model scripts (e.g., random_forest_heart.py) to train and evaluate predictions.

python random_forest_heart.py


📈 Key Findings

Geographic Independence: Analysis showed that patient location (Country/Continent) had no significant impact on heart attack risk.

Imbalance Impact: Initial models achieved high accuracy but low recall (missing sick patients). Balancing the data using SMOTE/Class Weights significantly improved the identification of at-risk patients.

📁 File Structure

eda_heart_analysis.py: Main script for cleaning, feature engineering, and SMOTE balancing.

heart_prediction_model.py: Logistic Regression implementation.

random_forest_heart.py: Random Forest implementation.

decision_tree_heart.py: Decision Tree implementation.

knn_heart.py: k-NN implementation.
