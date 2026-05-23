# Telco Customer Churn Analysis

## Overview
This project focuses on predicting customer churn for a telecommunications company using machine learning. The goal is to identify customers likely to leave and understand the key drivers behind churn behavior. The insights generated can help businesses improve customer retention strategies and reduce revenue loss.
The project follows an end-to-end data science workflow including data preprocessing, exploratory data analysis (EDA), feature engineering, model building, evaluation, and interpretation.
## Business Objective
•	Predict whether a customer will churn or not

•	Identify key factors influencing customer churn 

•	Improve customer retention through data-driven insights 

•	Compare multiple machine learning models for best performance 

## Dataset
The dataset used in this project is the **Telco Customer Churn** dataset, originally provided by IBM Sample Analytics Datasets. It contains customer demographic information, account details, and service usage behavior.

* **Source:** [Kaggle - Telco Customer Churn by BlastChar](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

Key features include:

•	Tenure

•	Monthly Charges

•	Total Charges

•	Contract Type 

•	Internet Service 

•	Payment Method 

Target variable: Churn (Yes/No) 

## Workflow
### 1. Data Preprocessing
   
•	Handling missing values 

•	Encoding categorical variables 

•	Feature scaling where necessary 

### 2. Exploratory Data Analysis (EDA)

•	Churn distribution analysis 

•	Correlation analysis 

•	Visualization of key customer patterns 

### 3. Feature Engineering

•	Transformation of categorical variables 

•	Selection of relevant predictors 

### 4. Model Building

The following models were implemented:

•	Logistic Regression

•	Decision Tree 

•	Random Forest 

•	XGBoost 

### 5. Model Evaluation. 

Models were evaluated using:

•	Accuracy 

•	Precision 

•	Recall 

•	F1-score 

•	ROC-AUC 

### 6. Hyperparameter Tuning
   
Optimized XGBoost model using hyperparameter tuning to improve predictive performance.

### 7. Model Interpretation
    
## •	Feature importance analysis 

<img width="616" height="292" alt="image" src="https://github.com/user-attachments/assets/2f26a5ac-57ad-4c44-b9fa-bc8737721db9" />


#### Feature Importance Visualization

The feature importance visualization highlights the variables that contributed most strongly to customer churn prediction within the Random Forest model.

Customer tenure emerged as the most influential feature, indicating that customer loyalty duration plays a critical role in retention behavior.

Pricing-related variables such as TotalCharges and MonthlyCharges also demonstrated substantial predictive influence, suggesting that pricing sensitivity contributes significantly to churn risk.

Contract duration and value-added support services further influenced churn prediction, emphasizing the importance of customer engagement and long-term service relationships.

## •	ROC curve comparison 

<img width="514" height="293" alt="image" src="https://github.com/user-attachments/assets/8fe41b64-4cf9-4eda-a244-7ee78889e9f1" />

#### ROC Curve Interpretation

The ROC curves demonstrate that Logistic Regression, Random Forest, and XGBoost achieved strong classification performance and maintained high discrimination capability between churn and non-churn customers.

XGBoost achieved the highest ROC-AUC score, followed closely by Random Forest and Logistic Regression.

The Decision Tree model demonstrated comparatively lower ROC-AUC performance, indicating reduced overall discrimination capability.


#### Model Performance Summary
The tuned XGBoost model achieved the best performance with a ROC-AUC score of approximately 0.848, indicating strong ability to distinguish between churners and non-churners.

#### Key Insights
•	Customers with month-to-month contracts are more likely to churn 
•	Higher monthly charges increase churn probability 
•	Customers with short tenure are at higher risk of leaving 
•	Certain payment methods are associated with higher churn rates 

#### Results Visualization
•	ROC Curve comparison across models 
 
•	Feature importance plots for interpretability 
 
## Business Insights & Recommendations

Based on the feature importance analysis and model predictions, the following strategic actions are recommended to mitigate customer retention risks:

* **Incentivize Contract Migrations:** Shift high-risk month-to-month customers toward 1-year or 2-year agreements by offering introductory annual discounts.
* **Promote Autopay Adoption:** Reduce billing friction by offering a one-time credit for switching from electronic checks to automated credit card/bank billing.
* **Proactive Retention Alerts:** Integrate the XGBoost/Random Forest model into customer workflows to flag high-risk accounts early, enabling the customer success team to intervene before cancellations occur.

# Tools & Technologies

•	Python 

•	Pandas & NumPy 

•	Scikit-learn 

•	XGBoost 

•	Matplotlib & Seaborn 

•	Jupyter Notebook


