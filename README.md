# Customer Conversion Prediction for Marketing Campaigns
## Overview

This project demonstrates how machine learning can be applied to predict customer conversion probability in a marketing context.

The goal is to identify which users are most likely to convert after interacting with a campaign, enabling more efficient targeting, reduced marketing costs, and improved return on investment (ROI).

## Business Context

NovaRetail, a mid-sized e-commerce company, runs marketing campaigns across multiple channels (email, social media, and paid ads).

However, campaigns are currently applied uniformly to all users, leading to inefficient budget allocation and missed opportunities.

This project addresses this problem by building a predictive model to estimate customer conversion probability and support data-driven marketing decisions.

## Objectives
Predict whether a customer will convert (converted = 1)
Build an end-to-end machine learning pipeline
Optimize model performance using hyperparameter tuning
Compare different models (Logistic Regression vs Random Forest)
Translate predictions into actionable business insights

## Dataset

A synthetic but realistic dataset was generated to simulate real-world marketing data.

Features include:
Demographics: age, income, city tier
Behavioral data: website visits, session duration, previous purchases
Marketing interactions: email clicks, ad clicks, campaign type
Commercial variables: discount percentage, product price
Target variable:
converted → whether the user made a purchase

## Machine Learning Workflow
1. Data Loading & Inspection

Explored dataset structure, missing values, and distributions.

2. Train/Test Split

Split data into training and test sets using stratification.

3. Preprocessing
Missing value handling (SimpleImputer)
Feature scaling (StandardScaler)
Encoding categorical variables (OneHotEncoder)
Combined using ColumnTransformer
4. Pipeline Construction

Built an end-to-end pipeline including preprocessing, feature selection, and model.

5. Model Training

Trained a baseline Logistic Regression model.

6. Model Evaluation

Evaluated using:

Accuracy
Confusion Matrix
Classification Report
ROC-AUC
7. Hyperparameter Tuning

Used GridSearchCV with cross-validation to optimize:

number of features (k)
regularization strength (C)
solver
8. Final Model Evaluation

Evaluated the tuned model on unseen test data.

9. Business Interpretation

Translated model outputs into marketing actions and strategy.

10. Model Comparison

Compared Logistic Regression with Random Forest to assess performance vs interpretability.

## Visualizations

The project includes key visualizations to evaluate model performance:

Confusion Matrix
ROC Curve
Precision-Recall Curve
Feature Importance (Random Forest)
Logistic Regression Coefficients

## Models Used
Logistic Regression
Interpretable baseline model
Provides direction and strength of feature impact (coef_)
Suitable for business understanding and explainability
Random Forest
Captures non-linear relationships and feature interactions
Provides feature importance rankings (feature_importances_)
Used to compare performance against Logistic Regression

## Results
The tuned model improved performance compared to the baseline
ROC-AUC demonstrated strong ability to distinguish converting vs non-converting users
Random Forest achieved competitive performance, suggesting non-linear effects in user behavior

## Business Impact

The model enables:

1. Targeting high-probability customers
2. Reducing wasted marketing spend
3. Increasing conversion rates
4. Data-driven campaign optimization

Instead of applying campaigns to all users, companies can prioritize high-value segments based on predicted conversion probability.

## Next Steps
Test advanced models (e.g., Gradient Boosting, XGBoost)
Incorporate real-world datasets
Deploy the model for real-time predictions
Integrate with A/B testing for campaign optimization
Extend the project to customer segmentation and lifetime value prediction

## Author
Andrea S. Greco
