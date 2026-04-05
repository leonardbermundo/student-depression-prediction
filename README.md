# 🧠 Student Depression Prediction

A machine learning project that predicts student depression risk using survey-based data, with a focus on identifying high-risk individuals through classification models and evaluation metrics.

---

## 📌 Overview
This project applies supervised machine learning techniques to analyze student lifestyle, academic, and financial factors to predict the likelihood of depression. The goal is to support early identification of at-risk students and enable data-driven mental health interventions.

---

## ⚙️ Tech Stack
- **Programming:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, LightGBM  
- **Techniques:** Data preprocessing, feature engineering, model evaluation  
- **Imbalance Handling:** BorderlineSMOTE  

---

## 📊 Methodology

### 1. Data Preparation
- Cleaned and preprocessed survey dataset  
- Handled missing values and encoded categorical variables  

### 2. Exploratory Data Analysis (EDA)
- Analyzed distributions and relationships between variables  
- Identified potential predictors of depression risk  

### 3. Model Development
- Implemented classification models:
  - Logistic Regression  
  - K-Nearest Neighbors (KNN)  
  - Random Forest  
  - Gradient Boosting  
  - LightGBM  

### 4. Model Evaluation
- Evaluated models using:
  - Recall (priority metric for detecting high-risk cases)  
  - ROC-AUC  

### 5. Model Optimization
- Applied hyperparameter tuning  
- Addressed class imbalance using BorderlineSMOTE  

---

## 🏆 Results
- **Best Model:** Logistic Regression (with BorderlineSMOTE + tuning)  
- **Recall:** 88.90%  
- **ROC-AUC:** 91.75%

👉 Recall was prioritized to minimize false negatives, ensuring high-risk individuals are not missed.

---

## 🔍 Key Insights
- Academic pressure and financial stress are the strongest predictors of depression risk  
- Prioritizing recall improves identification of high-risk individuals  

---

## 📊 Visualizations

### Model Performance
![Model Performance](docs/images/model_performance.png)

### SHAP Summary Plot
![SHAP Summary](docs/images/shap_summary.png)

---
