# Telco-Customer-Churn-Analysis


Data Analyst Project Report

Project Type: Customer Churn Analysis and Machine Learning  
Tools: Python, Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn, LightGBM  

## Project Objective

The objective of this project is to analyze customer churn, identify factors associated with customers leaving the telecom service, and develop machine learning models to predict potential customer churn.  

## Dataset Overview

The dataset contains 7,043 customer records and 21 columns, covering customer demographics, services, contract types, payment methods, tenure, and charges. The target variable is Churn.  

## Data Cleaning and Preparation
Removed the customerID column.  
Converted TotalCharges to numeric format.  
Replaced 11 blank TotalCharges values with the median.  
Encoded categorical variables using LabelEncoder.  
Applied StandardScaler to numerical features.  
Split the data into 75% training and 25% testing sets.  

## Exploratory Data Analysis (EDA)

The dataset contains 1,869 customers who churned and 5,174 who did not, corresponding to an overall churn rate of approximately 26.5%.  

The analysis examined numerical distributions, correlations, and relationships between customer characteristics and churn. Tenure, contract type, online security, and technical support showed notable relationships with churn. Gender showed relatively little difference in churn risk.  

## Machine Learning Models

Three classification models were trained and evaluated.  

Model	Accuracy	Churn Recall	Churn F1-Score  
LightGBM	80%	52%	0.57  
Decision Tree	78%	35%	0.45  
Logistic Regression	80%	52%	0.57  

##Key Findings
LightGBM and Logistic Regression achieved the highest reported accuracy at 80%.  
Decision Tree achieved 78% accuracy but had lower churn recall.  
LightGBM and Logistic Regression identified 52% of actual churn cases in the test set.  
The target classes are imbalanced, with more non-churning customers than churning customers.  

## Business Recommendations
Identify customers with short tenure and improve their early customer experience.  
Investigate the relationship between contract types and customer churn.  
Evaluate how technical support and online security services relate to customer retention.  
Develop targeted retention campaigns for customers identified as high risk.  
Improve model recall to identify more customers likely to churn.  

## Conclusion

This project demonstrates how Python and machine learning can be used to analyze customer churn and predict customer behavior. LightGBM and Logistic Regression achieved 80% accuracy, with a churn F1-score of 0.57.  
