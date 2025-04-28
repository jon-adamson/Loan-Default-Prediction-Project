# Loan Default Prediction

## 📚 Overview
Predicting loan default is a critical task for financial institutions to manage risk and minimize losses.  
In this project, I build machine learning models to predict whether a borrower will default on a loan, based on their financial and personal information.

---

## 🎯 Problem Statement
Financial institutions lose billions each year due to loan defaults.  
Accurately predicting which borrowers are likely to default enables better decision-making, reduces risk, and improves profitability.

---

## 🛠️ Tools & Technologies
- Python (Pandas, NumPy, Scikit-learn, XGBoost, imbalanced-learn)  
- Matplotlib, Seaborn (visualizations)  
- SHAP (model explainability)  
- Streamlit (optional: web app)  
- Jupyter Notebook  

---

## 📈 Project Workflow

### 1. Data Collection
- Used LendingClub Loan Dataset from Kaggle.
- Focused on loans issued in 2018.

### 2. Data Cleaning
- Handled missing values through imputation and feature removal.
- Created a binary target variable: `1 = Default`, `0 = Fully Paid`.

### 3. Exploratory Data Analysis (EDA)
- Analyzed borrower features: loan amount, income, credit score, employment length.
- Visualized default rates across key borrower segments.

### 4. Model Building
- Built baseline Logistic Regression model.
- Developed tree-based models (Random Forest, XGBoost).
- Handled class imbalance using SMOTE and class weight adjustments.

### 5. Model Evaluation
- Evaluated models using Precision, Recall, F1-Score, and ROC-AUC.
- Visualized ROC and Precision-Recall curves.

### 6. Model Interpretation
- Analyzed feature importance to identify key drivers of loan default.
- Applied SHAP to explain individual model predictions.

### 7. Business Recommendations
- Proposed strategies for risk mitigation based on model outputs.
- Suggested using model scores to enhance underwriting processes.

---

## 📊 Key Results
- XGBoost achieved an ROC-AUC score of **0.84** on the test set.
- Top predictors of default:
  - Credit score
  - Debt-to-income ratio
  - Loan amount
  - Employment length

---

## 🚀 Future Work
- Incorporate behavioral data (e.g., payment history over time).
- Build a live Streamlit app for real-time loan risk scoring.
- Explore cost-sensitive learning to minimize false negatives.

---

## 📂 Project Structure

