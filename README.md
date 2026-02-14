# Customer Churn Prediction – Comparative Machine Learning Study

## Overview

This project presents a structured and comparative machine learning study for predicting customer churn in the banking sector. The objective is to build an interpretable, statistically validated, and business-aligned churn prediction framework.

The workflow includes:

- Data inspection  
- Exploratory Data Analysis (EDA)  
- Feature engineering  
- Model benchmarking  
- Cross-validation  
- Hyperparameter tuning  
- Pipeline-based implementation for reproducibility  

---

## Dataset

The dataset contains **10,000 customer records** with 12 features, including:

- Customer demographics (age, gender, country)
- Financial indicators (credit score, balance, estimated salary)
- Engagement features (tenure, products number, credit card status, active membership)
- Target variable: `churn` (binary classification)

### Key Observations

- No missing values  
- Class imbalance: ~80% non-churn, ~20% churn  
- Mixed numerical and categorical features  
- Suitable for structured preprocessing pipelines  

---


## Methodology

### 1. Data Preprocessing

- Stratified train-test split  
- OneHotEncoding for categorical variables  
- Feature scaling (StandardScaler / MinMaxScaler)  
- ColumnTransformer for structured transformations  
- Full modeling pipeline using `sklearn.pipeline.Pipeline`  

---

### 2. Exploratory Data Analysis

- Numerical feature distributions  
- Churn-wise comparisons  
- Country and gender analysis  
- Correlation analysis  
- Class imbalance visualization  

---

### 3. Models Compared

The following classification algorithms were benchmarked:

- Logistic Regression  
- Random Forest  
- Gradient Boosting  
- Support Vector Machine (SVC)  
- AdaBoost  
- Gaussian Naive Bayes  

All models were evaluated under consistent preprocessing conditions.

---

### 4. Model Evaluation

Evaluation metrics used:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- ROC-AUC  
- Confusion Matrix  
- Classification Report  
- Stratified K-Fold Cross Validation  
- GridSearchCV for hyperparameter tuning  

Special attention was given to **Recall and ROC-AUC** due to class imbalance.

---

## Key Results

- Confirmed moderate class imbalance (~20% churn)
- Tree-based models outperform linear baselines
- Gradient Boosting and Random Forest show strong ROC-AUC performance
- Cross-validation improves robustness
- Pipeline implementation ensures reproducibility

Target benchmark: **ROC-AUC > 0.90** (model dependent).

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Joblib  

---

## Business Relevance

Customer retention is significantly more cost-effective than acquisition. This framework supports:

- Early churn detection  
- Customer risk scoring  
- Targeted retention strategies  
- Data-driven decision-making  

The study bridges predictive modeling with business-oriented evaluation.

---

## Future Improvements

- SHAP-based interpretability  
- Cost-sensitive learning  
- Threshold optimization  
- Model ensembling  
- Deployment via Streamlit or Flask  
- Interactive dashboard integration  

---

## About Me
Anuj Jain

B.Tech (Electronics and Communication Engineering),

Rajasthan Technical University, Kota

Research Interests: Machine Learning, Data Science, Decision Analytics

LinkedIn: https://www.linkedin.com/in/anujjain9

Email: anuj962005@gmail.com
