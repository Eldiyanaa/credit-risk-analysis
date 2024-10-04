# Credit Risk Analysis and Modeling

## Overview

This project focuses on building a Credit Scoring Model to assess and classify users into different risk categories (high risk or low risk) based on their likelihood of defaulting on a loan. This is a challenge project for 10 Academy Week 6, which involves data exploration, feature engineering, model development, and deploying a machine learning model as an API.

---

## Problem Statement

Bati Bank, a leading financial service provider, is partnering with an eCommerce company to offer a buy-now-pay-later service. The goal is to create a **Credit Scoring Model** that predicts a customer's risk of default and assigns credit scores to potential borrowers.

---

## Objectives

1. Define a proxy variable to categorize users into high or low risk.
2. Select features that are good predictors of the default risk.
3. Develop a model that assigns risk probability to new customers.
4. Predict the optimal loan amount and duration based on the customer’s risk.
5. Deploy the trained machine learning model via a REST API for real-time predictions.

---

## Dataset

The dataset used for this project contains transaction data from the eCommerce platform. Some key features include:
- `TransactionId`
- `AccountId`
- `Amount`
- `ProductCategory`
- `TransactionStartTime`
- `FraudResult`

---

## Tasks

### **Task 1: Understanding Credit Risk**
- Research the concept of credit risk, particularly as it applies to the Basel II Capital Accord.
- Identify important predictors of default risk.

### **Task 2: Exploratory Data Analysis (EDA)**
- Understand the structure of the dataset, including columns and data types.
- Compute summary statistics to examine central tendencies and variabilities.
- Analyze the distribution of numerical and categorical features.
- Perform correlation analysis between numerical variables.
- Detect missing values and outliers.

### **Task 3: Feature Engineering**
- Create new features such as aggregate transaction statistics (sum, average).
- Extract date-time features such as the transaction hour, day, month.
- Encode categorical variables using one-hot encoding and label encoding.
- Handle missing values using imputation techniques.

### **Task 4: Modeling**
- Split the data into training and test sets.
- Choose and train models, including Logistic Regression, Decision Trees, and Random Forest.
- Perform hyperparameter tuning to improve model performance.
- Evaluate model performance using metrics such as Accuracy, Precision, Recall, F1 Score, and ROC-AUC.

### **Task 5: Model Serving API**
- Develop a REST API using Flask or FastAPI to serve the trained models for real-time predictions.
- Deploy the API for public use.

---

## Skills and Tools

- **Python Packages**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Machine Learning**: Logistic Regression, Decision Trees, Random Forests, Hyperparameter Tuning
- **CI/CD**: GitHub Actions
- **MLOps**: MLFlow, Model Management, API Deployment with Flask/FastAPI

---

## Usage

1. Clone this repository:
   ```bash
   git clone git@github.com:Eldiyanaa/credit-risk-analysis.git
2. Install dependencies:
  ```bash
   pip install -r requirements.txt
3. Run the model training script:
  ```bash
   python src/train_model.py
4. Serve the model using Flask:
  ```bash
   python src/app.py
