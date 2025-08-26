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

# Task 3: Energy Consumption Forecasting

## Objective
The objective of this task is to forecast short-term household energy consumption using historical data.  
This is a time series forecasting problem where we compare multiple models to identify which method works best.

## Approach
1. Loaded the **Household Power Consumption dataset** from the UCI Machine Learning Repository.  
2. Selected the `Global_active_power` column as the target variable.  
3. Filtered the data to two years (2007–2008) for faster training and resampled it to daily averages.  
4. Split the dataset into training and testing sets (last 90 days used for testing).  
5. Trained three models:  
   - **ARIMA (statsmodels)** for baseline time series forecasting.  
   - **Prophet** for handling seasonality and trend.  
   - **XGBoost** with lag features for machine learning based forecasting.  
6. Evaluated the models using **MAE (Mean Absolute Error)** and **RMSE (Root Mean Squared Error)**.  
7. Visualized actual vs forecasted values to compare model performance.

## Results and Findings
- **ARIMA** provided a reasonable baseline but struggled with complex variations.  
- **Prophet** captured trends and seasonality better than ARIMA.  
- **XGBoost** gave the best overall accuracy when lag features were added.  
- Overall, XGBoost proved to be the most effective approach for forecasting short-term household energy consumption.  

