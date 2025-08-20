# DevelopersHub_Internship_Tasks
# Task 1: Term Deposit Subscription Prediction (Bank Marketing)

## Objective
Predict whether a bank customer will subscribe to a term deposit using classification models.

## Approach
1. Loaded and explored the Bank Marketing dataset (small version ~4k rows).
2. Encoded categorical features using Label Encoding.
3. Split data into training (80%) and testing (20%).
4. Trained Logistic Regression (scaled features) and Random Forest (unscaled).
5. Evaluated models using Confusion Matrix, F1-Score, and ROC Curve.
6. Applied SHAP to explain predictions and identify key features.

## Results and Findings
- Dataset is imbalanced: more customers said "No" than "Yes".
- Random Forest performed better than Logistic Regression.
- Important features for prediction:
  - Call duration
  - Previous campaign outcome
  - Age
  - Account balance

