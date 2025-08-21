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


# Task 2: Customer Segmentation (K-Means Clustering)

## Objective
The objective of this task is to group customers into segments based on their annual income and spending score.  
This helps in understanding different customer profiles and designing targeted marketing strategies.

## Approach
1. Loaded the **Mall Customers dataset** containing CustomerID, Gender, Age, Annual Income, and Spending Score.  
2. Performed exploratory data analysis (EDA) to understand the distribution of income, age, and spending.  
3. Selected **Annual Income** and **Spending Score** as key features for clustering.  
4. Applied **K-Means clustering** after scaling the features.  
5. Used the **Elbow Method** to determine the optimal number of clusters.  
6. Visualized clusters using scatter plots and **PCA (dimensionality reduction)**.  
7. Analyzed each cluster and proposed suitable marketing strategies.  

## Results and Findings
- The dataset was successfully divided into **5 customer clusters**.  
- Identified different customer groups, such as:  
  - High income, high spenders (premium customers)  
  - High income, low spenders (potential luxury segment)  
  - Low income, high spenders (value-seekers)  
  - Low income, low spenders (budget-conscious)  
  - Moderate income, moderate spenders (upsell opportunities)  
- Example marketing strategies:  
  - Target high spenders with premium offers  
  - Engage low spenders with discounts or loyalty programs  
  - Upsell to middle segment with bundles and cross-selling  

Overall, clustering helped in understanding customer behavior patterns and provided actionable insights for marketing strategy.

