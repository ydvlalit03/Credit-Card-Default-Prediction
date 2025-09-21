# Credit Card Default Prediction 🔮💳

This project predicts the likelihood of a customer defaulting on their credit card payments using **machine learning models**.  
It applies **data cleaning, exploratory data analysis (EDA), feature engineering, class imbalance handling, and model tuning** to build an accurate and business-relevant solution for financial institutions.

---

## 📌 Project Overview
Credit card defaults are a major concern for banks and lenders. Accurate prediction models can help reduce risk and improve decision-making.  
This study builds a **classification pipeline** to predict whether a customer will default in the next billing cycle.

---

## 🛠 Methodology
1. **Data Cleaning**
   - Imputed missing values (e.g., AGE column using median).
   - Fixed invalid categorical labels in `MARRIAGE` and `EDUCATION`.
   - Treated outliers using **capping (winsorization)**.

2. **Exploratory Data Analysis (EDA)**
   - Analyzed target distribution (class imbalance ~19% defaulters).
   - Studied relationships between **age, marital status, education, credit limit, bills, and payments**.
   - Identified repayment history as a strong predictor.

3. **Feature Engineering**
   - Created **credit utilization ratio, delinquency metrics, repayment gaps, payment trends, and demographic interactions**.
   - Improved correlation with target variable.

4. **Class Imbalance Handling**
   - Used **SMOTE (Synthetic Minority Oversampling Technique)** to balance classes.

5. **Feature Selection**
   - Selected **Top 20 features** using Random Forest importance.

6. **Model Training**
   - Models: Logistic Regression, Decision Tree, Random Forest, AdaBoost, Gradient Boosting, XGBoost, KNN.
   - **GridSearchCV** used for hyperparameter tuning.
   - Evaluation metrics: **Accuracy, Precision, Recall, F1, F2, ROC-AUC**.

7. **Threshold Adjustment**
   - Optimized decision threshold to prioritize **recall (catching defaulters)** over accuracy.

---

## 📊 Results
- **Best Model:** Tuned **Random Forest**  
- **Performance (Test Set):**
  - Accuracy: **88.57%**
  - Precision: **91.90%**
  - Recall: **84.98%**
  - F1 Score: **88.30%**
  - F2 Score: **86.28%**
  - ROC-AUC: **0.9485**

This model strikes a balance between **business needs** (minimizing missed defaulters) and **predictive accuracy**.

---

## 📂 Repository Structure
