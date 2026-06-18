# 📉 Telecom Customer Churn Prediction & Retention Strategy

## 🎯 Executive Summary
Customer retention is a cornerstone of sustainable business growth. This project tackles the challenge of customer attrition in the telecommunications sector by building and evaluating multiple machine learning classification models. Beyond just predicting *who* will leave, this project translates statistical probabilities into a concrete, ROI-positive **Retention Marketing Strategy**, demonstrating a seamless bridge between advanced data science and actionable business strategy.

## 🛠️ Analytical Approach & Machine Learning Models
* **Core Technologies:** R, Tidyverse, caret, glmnet, pROC, MASS, e1071, tree.
* **Feature Engineering & EDA:** Conducted extensive exploratory data analysis, transformed categorical variables, and applied log/square-root transformations to normalize continuous financial variables (Tenure, Total Charges).
* **Predictive Modeling:** Trained, cross-validated, and optimized five distinct classification algorithms to identify at-risk customers:
  * **Logistic Regression** *(Selected for business deployment: Highest AUC of 0.848)*
  * **Decision Trees** *(Highest raw test accuracy: 79% after pruning)*
  * **Linear Discriminant Analysis (LDA)**
  * **Quadratic Discriminant Analysis (QDA)**
  * **Naive Bayes**

## 📊 Key Drivers of Customer Churn
By analyzing the coefficients of the optimized Logistic Regression model, several critical behavioral insights were uncovered:
* **Contract Elasticity:** Customers on two-year agreements are significantly less likely to churn compared to month-to-month users.
* **Service Friction:** Fiber Optic internet users exhibited higher churn rates than DSL users, indicating a need for targeted service quality interventions.
* **Payment Friction:** Electronic check users and paperless billing adopters showed elevated risk, while automated payments increased retention.

## 💡 Business Value & Marketing ROI
*This project goes beyond predictive modeling by calculating the direct financial impact of marketing interventions.*

* **The Problem:** The model identified 154 high-risk customers, representing a potential **$11,988.20** in lost monthly recurring revenue (MRR).
* **The Strategy:** Proposed a targeted promotional campaign offering a $15/month incentive for 3 months to secure short-term loyalty and transition users past the high-risk churn window.
* **The ROI:** With a calculated intervention cost of $6,930, the strategy successfully protects $35,964.60 in at-risk revenue, generating a **net financial benefit of $29,034.60** for the quarter. This methodology is directly applicable to optimizing Customer Acquisition Cost (CAC) and maximizing Customer Lifetime Value (CLV) in media and marketing analytics.
