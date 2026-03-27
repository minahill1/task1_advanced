# 🔄 End-to-End ML Pipeline for Customer Churn Prediction

A production-ready machine learning pipeline that predicts customer churn using the Telco Customer Churn dataset. This project demonstrates best practices for building reusable, scalable ML pipelines using Scikit-learn's Pipeline API with comprehensive preprocessing, model training, hyperparameter tuning, and model export functionality.

## 🎯 Project Overview

This project builds a complete ML pipeline that predicts whether a customer will churn (cancel their subscription) based on demographic, account, and service usage data. The pipeline handles all aspects of the machine learning workflow:

- **Data Preprocessing**: Automated handling of missing values, categorical encoding, and feature scaling
- **Feature Engineering**: Intelligent transformation of features for optimal model performance
- **Model Training**: Multiple algorithms with hyperparameter optimization
- **Model Evaluation**: Comprehensive metrics and visualizations
- **Model Export**: Production-ready serialization using joblib

## ✨ Features

- **Complete ML Pipeline**: End-to-end automation from raw data to predictions
- **Smart Preprocessing**: 
  - Automatic detection of numeric and categorical columns
  - Multiple encoding strategies (One-Hot, Ordinal, Label Encoding)
  - Feature scaling with StandardScaler and RobustScaler
  - Missing value handling with SimpleImputer
- **Multiple Models**: Logistic Regression, Random Forest, XGBoost, and Gradient Boosting
- **Hyperparameter Tuning**: GridSearchCV and RandomizedSearchCV with cross-validation
- **Model Persistence**: Export entire pipeline using joblib for production deployment
- **Comprehensive Evaluation**: Accuracy, precision, recall, F1-score, ROC-AUC, confusion matrix
- **Feature Importance**: Visualization of top predictive features

## 🛠️ Technologies Used

- **Python 3.8+**
- **Scikit-learn** - Pipeline, preprocessing, models, tuning
- **Pandas & NumPy** - Data manipulation
- **Matplotlib & Seaborn** - Visualization
- **XGBoost** - Advanced gradient boosting
- **Joblib** - Model serialization
- **Imbalanced-learn** - Handling class imbalance
- **SHAP** - Model interpretability (optional)

## 📊 Dataset

The project uses the **Telco Customer Churn Dataset**:

### Dataset Statistics
- **Samples**: 7,043 customers
- **Features**: 21 columns (20 predictors, 1 target)
- **Target**: Churn (Yes/No)
- **Churn Rate**: ~26.5% (imbalanced dataset)

### Features Description

| Feature | Type | Description |
|---------|------|-------------|
| customerID | ID | Unique customer identifier |
| gender | Categorical | Male/Female |
| SeniorCitizen | Binary | 1 if senior, 0 otherwise |
| Partner | Binary | Whether customer has a partner |
| Dependents | Binary | Whether customer has dependents |
| tenure | Numeric | Months customer has stayed |
| PhoneService | Binary | Whether customer has phone service |
| MultipleLines | Categorical | Phone service lines |
| InternetService | Categorical | DSL, Fiber optic, or No |
| OnlineSecurity | Categorical | Whether customer has online security |
| OnlineBackup | Categorical | Whether customer has online backup |
| DeviceProtection | Categorical | Whether customer has device protection |
| TechSupport | Categorical | Whether customer has tech support |
| StreamingTV | Categorical | Whether customer streams TV |
| StreamingMovies | Categorical | Whether customer streams movies |
| Contract | Categorical | Month-to-month, One year, Two year |
| PaperlessBilling | Binary | Whether customer uses paperless billing |
| PaymentMethod | Categorical | Payment method used |
| MonthlyCharges | Numeric | Monthly charges amount |
| TotalCharges | Numeric | Total charges amount |
| Churn | Target | Yes/No (target variable) |

## 🚀 Installation

### Prerequisites
- Python 3.8 or higher
- 4GB+ RAM recommended
- Git

### Setup Instructions

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/churn-prediction-pipeline.git
cd churn-prediction-pipeline
