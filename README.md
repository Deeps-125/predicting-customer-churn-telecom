 Telecom Customer Churn Prediction

## Project Overview

Customer churn is an important challenge for telecommunication companies. When customers discontinue their services, the company may lose recurring revenue and spend additional resources on acquiring new customers.

This project uses machine learning to analyze customer information and predict whether a customer is likely to churn.

## Business Problem

The objective is to identify customers who are likely to leave the telecom service based on their demographic information, service usage, contract details, and billing information.

Early identification of potential churn customers can help a telecom company understand customer behavior and plan appropriate customer retention strategies.

## Project Goals

* Analyze customer demographics and service-related information.
* Clean and preprocess the customer data.
* Perform Exploratory Data Analysis (EDA).
* Identify patterns associated with customer churn.
* Prepare features for machine learning.
* Build multiple classification models.
* Evaluate model performance using different metrics.
* Identify important factors related to customer churn.

## Dataset

The project uses the **Telco Customer Churn** dataset.

The dataset contains information related to:

* Customer demographics
* Gender and senior citizen status
* Partner and dependents
* Tenure
* Phone and internet services
* Contract type
* Payment method
* Monthly charges
* Total charges
* Churn status

### Target Variable

**Churn**

* `0` → No Churn
* `1` → Churn

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Imbalanced-learn
* SHAP

## Project Workflow

### 1. Data Collection

The dataset is loaded from the CSV file:

`WA_Fn-UseC_-Telco-Customer-Churn.csv`

### 2. Data Cleaning and Preprocessing

The following preprocessing steps are performed:

* Convert `TotalCharges` into numeric format.
* Handle missing values.
* Convert the `Churn` column from `Yes/No` into `1/0`.
* Remove unnecessary columns.
* Convert categorical variables into numerical features.
* Scale features for Logistic Regression.

### 3. Exploratory Data Analysis

EDA is performed to understand:

* Numerical feature distributions.
* Churn distribution.
* Internet service categories.
* Customer and service-related patterns.
* Relationships between features and churn.

### 4. Feature Engineering

Features are separated from the target variable, categorical variables are encoded, and the dataset is prepared for machine learning.

### 5. Train-Test Split

The dataset is divided into training and testing datasets.

The training data is used to train the machine learning models, while the testing data is used to evaluate their performance.

### 6. Model Building

Four machine learning classification models are trained:

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. XGBoost

### 7. Model Evaluation

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC
* Confusion Matrix
* Classification Report

## Machine Learning Models

### Logistic Regression

Used as a baseline classification model for predicting customer churn.

### Decision Tree

A tree-based classification model that makes predictions using decision rules based on customer features.

### Random Forest

An ensemble learning algorithm that combines multiple decision trees to improve predictive performance.

### XGBoost

A gradient boosting algorithm used for classification and capable of handling complex relationships between features.

## Results

Model performance will be compared using Accuracy, F1-Score, ROC-AUC, Precision, and Recall.

The final model can be selected based on the evaluation results and the business objective of identifying potential churn customers.

## Key Insights

The analysis helps understand how factors such as:

* Contract type
* Tenure
* Monthly charges
* Internet service
* Payment method
* Customer services

may be associated with customer churn.

## Future Improvements

* Hyperparameter tuning.
* Cross-validation.
* Advanced feature engineering.
* Threshold optimization.
* Model explainability using SHAP.
* Deployment as a web application or API.
* Monitoring model performance after deployment.

## How to Run

### 1. Clone or download the repository.

### 2. Open the Jupyter Notebook in Google Colab or Jupyter Notebook.

### 3. Upload the dataset:

`WA_Fn-UseC_-Telco-Customer-Churn.csv`

### 4. Install required libraries if needed:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn shap
```

### 5. Run the notebook cells sequentially.

## Project Structure

```text
Telco-Customer-Churn/
│
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
├── Telco_Customer_Churn.ipynb
├── README.md
└── requirements.txt
```

## Conclusion

This project demonstrates an end-to-end machine learning workflow for customer churn prediction, starting from data collection and preprocessing through exploratory analysis, model building, and model evaluation.

The project provides a practical example of how machine learning can be applied to customer churn analysis in the telecommunications domain.

