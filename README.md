# 💳 Loan Default Prediction Using LendingClub Data

This project builds machine learning models to predict whether a borrower will **default** on a loan or **fully repay** it, using 2018 data from LendingClub. The workflow includes data cleaning, exploratory data analysis (EDA), feature engineering, model training (Logistic Regression, Random Forest, XGBoost), and model interpretation using SHAP values.

---

## 📌 Project Objective

Financial institutions face significant risk from loan defaults. The goal of this project is to create a reliable, interpretable model that can predict default risk at the time of loan application—helping lenders make smarter decisions and reduce financial losses.

---

## 🛠️ Tools & Libraries

- Python, Pandas, NumPy
- Scikit-learn, XGBoost
- Matplotlib, Seaborn
- SHAP (for model interpretation)
- imbalanced-learn (SMOTE)
- Jupyter Notebook

---

## 📊 Workflow Overview

### 1. Data Preparation
- Filtered LendingClub data to loans issued in **2018**
- Retained only **“Fully Paid”** and **“Charged Off”** loans
- Created binary target: `1 = default`, `0 = fully paid`
- Dropped post-loan outcome fields and high-NA columns
- Handled missing values with mode/median imputation

### 2. Exploratory Data Analysis (EDA)
- Plotted distributions (e.g., loan amount)
- Analyzed default rates across income brackets
- Visualized correlation heatmap of numeric features

### 3. Preprocessing
- One-hot encoded categorical features (e.g., grade, term, verification status)
- Used **SMOTE** to balance the training dataset

### 4. Model Training & Evaluation
- Trained three models:
  - Logistic Regression (baseline)
  - Random Forest
  - XGBoost
- Evaluated models with:
  - Precision, Recall, F1-Score
  - ROC-AUC
  - Confusion Matrix

### 5. Feature Importance
- Extracted feature importances from Random Forest and XGBoost
- Used **SHAP values** to interpret how features impact individual predictions

---

## 🔍 Key Insights

- **Top predictors** of default: `interest rate`, `loan grade`, `term`, `debt-to-income ratio`, and **recent credit inquiries**.
- The **XGBoost model** achieved the highest performance with a solid ROC-AUC score and improved recall.
- SHAP analysis showed `home_ownership_RENT`, `inq_last_6mths`, and `grade_B` had strong impact on prediction outcomes.

---

## 📁 Repository Structure




---

## 📌 Future Improvements

- Hyperparameter tuning (GridSearchCV)
- Deploy model using Streamlit for interactive scoring
- Add economic variables or credit bureau features for richer modeling

---

## 📬 Contact

Feel free to connect or reach out if you have questions!

**Jonathan Adamson**  
📧 jonathan.adamson324@gmail.com  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/jonathanmadamson/)  
