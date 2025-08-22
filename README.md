#  Bank Term Deposit Subscription Prediction

##  Objective
The goal of this project is to **predict whether a client will subscribe to a term deposit** based on the Bank Marketing dataset (UCI Machine Learning Repository).  
This is a binary classification problem (`yes` / `no`).

## Dataset
- **Source:** [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)
- File used: `bank-additional-full.csv`
- Rows: ~41k  
- Features: 20 input variables + target (`y`)

## Approach
1. **Data Preprocessing**
   - Handled categorical variables with one-hot encoding.
   - Normalized numerical features where needed.
   - Split into train/test sets.

2. **Models Implemented**
   - **Logistic Regression**
   - **Random Forest Classifier**

3. **Model Evaluation**
   - Accuracy
   - Confusion Matrix
   - Classification Report
   - SHAP values for explainability

##  Results
- **Logistic Regression Accuracy:** 0.912479%
- **Random Forest Accuracy:** 0.917456% 
- Random Forest showed stronger predictive power, especially in handling categorical features.
- SHAP analysis highlighted the most influential features (e.g., duration of last call, number of previous contacts, etc.).

##  Findings
- Campaign-related features (like `duration`, `previous`, `poutcome`) have strong influence.
- Random Forest outperformed Logistic Regression in capturing complex patterns.
- SHAP values provided interpretability, showing why the model made certain predictions.
