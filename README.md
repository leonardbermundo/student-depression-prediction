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


With the help of hyperparameter tuning and resampling (BorderlineSMOTE), recall improves to 88.90% for the holdout data.

<img width="418" height="66" alt="Screenshot 2026-04-05 at 11 14 02 PM" src="https://github.com/user-attachments/assets/828e09a5-197d-4ff1-bc15-459d6a4f88b3" />


#### Accuracy, Recall, and ROC-AUC (for holdout data)

<img width="131" height="113" alt="Screenshot 2026-04-05 at 11 17 39 PM" src="https://github.com/user-attachments/assets/843f8d8d-08cc-40bf-8889-298a5f903c57" />


#### Confusion Matrix

Out of 991 depressed students, **our model correctly identified 881**.

<img width="637" height="470" alt="image" src="https://github.com/user-attachments/assets/b955246a-61fa-46f2-a888-c1c1a17aabe2" />


#### Model Discrimination Performance

The model correctly identifies at-risk students from non at-risk students **91.75%** of the time.

<img width="606" height="590" alt="image" src="https://github.com/user-attachments/assets/ed2e83d3-e198-4b37-afae-bb18ba4f07ee" />


### SHAP Summary Plot
<img width="790" height="540" alt="image" src="https://github.com/user-attachments/assets/03d1333e-c630-469b-bcf6-d291f1cb4f51" />

<img width="771" height="540" alt="image" src="https://github.com/user-attachments/assets/ea4f9339-5dd6-43c8-90ff-6b898f45d568" />

---
