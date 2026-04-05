# 🧠 Student Depression Prediction

A machine learning project that predicts student depression risk using survey-based data, with a focus on identifying high-risk individuals through classification models and evaluation metrics.

---

## 📌 Overview
This project applies supervised machine learning techniques to analyze student lifestyle, academic, and financial factors to predict the likelihood of depression. 

The objective is to support **early identification of at-risk students** and enable **data-driven mental health interventions**.

---

## 📊 Dataset

The dataset used in this project was sourced from:

- [Kaggle - Student Depression Dataset](https://www.kaggle.com/datasets/hopesb/student-depression-dataset)

It includes demographic, academic, and lifestyle-related features such as academic pressure, financial stress, and study satisfaction. The target variable indicates whether a student is at risk of depression.

--

## ⚙️ Tech Stack
- **Programming:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, LightGBM, SHAP  
- **Techniques:** Data preprocessing, feature engineering, model evaluation  
- **Imbalance Handling:** BorderlineSMOTE  

---

## 📊 Methodology

### 1. Data Preparation
- Cleaned and preprocessed survey dataset
- Handled missing values and encoded categorical variables
- Applied feature scaling where necessary 

### 2. Exploratory Data Analysis (EDA)
- Analyzed distributions of key variables
- Identified relationships between features and depression risk
- Highlighted important patterns in academic and financial stress  

### 3. Feature Engineering
- Selected relevant predictors for modeling
- Transformed categorical variables for model compatibility

### 4. Model Development
- Implemented classification models:
  - Logistic Regression  
  - K-Nearest Neighbors (KNN)  
  - Random Forest  
  - Gradient Boosting  
  - LightGBM  

### 5. Model Evaluation
- Evaluated models using:
  - Recall (priority metric for detecting high-risk cases)  
  - ROC-AUC
 
👉 Recall was prioritized to minimize false negatives, ensuring high-risk individuals are not missed.

### 6. Model Optimization
- Applied hyperparameter tuning  
- Addressed class imbalance using BorderlineSMOTE  

---

## 🏆 Results
- **Best Model:** Logistic Regression
- **Enhancements:** BorderlineSMOTE + Hyperparameter tuning
- **Recall:** 88.90%  
- **ROC-AUC:** 91.75%

👉 Logistic Regression outperformed other models after optimization and class imbalance handling.

---

## 🔍 Model Interpretability
Used **SHAP (SHapley Additive exPlanations)** to interpret model predictions
Identified key drivers of depression risk:
- Academic Pressure
- Financial Stress

---

## 🔍 Key Insights
- Students experiencing high academic pressure and financial stress are significantly more likely to be at risk
- Handling class imbalance (SMOTE) improved model performance
- Prioritizing recall ensures better identification of vulnerable individuals

--- 

## 💡 Recommendations
- As a call to action, we are recommending for students to promote lifestyle & well-being through structured routines, implement campus wellness programs, improve access to counseling services and peer support groups, and to encourage healthy coping mechanisms. 

---

## 📊 Visualizations

### Model Performance


With the help of hyperparameter tuning and resampling (BorderlineSMOTE), recall improves to **88.90%** for the holdout data.

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
