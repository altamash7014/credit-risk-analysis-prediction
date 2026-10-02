# Credit Risk Analysis & Prediction Dashboard

## 📌 Project Overview

An end-to-end **Credit Risk Analysis and Prediction** project combining **Data Science and Data Analytics**.

The project analyzes loan applicant data, predicts the probability of loan default using machine learning, and presents the results through an interactive **Power BI credit-risk dashboard**.

The workflow covers:

**Data Cleaning → Feature Engineering → ML Modeling → Hyperparameter Tuning → Default Prediction → Risk Segmentation → Power BI Analytics**

---

## 🛠️ Tech Stack

- **Python** — Data cleaning, feature engineering and machine learning
- **Pandas & NumPy** — Data manipulation and preprocessing
- **Scikit-learn** — Preprocessing, Logistic Regression, Random Forest and model evaluation
- **XGBoost** — Credit default prediction
- **RandomizedSearchCV** — Hyperparameter tuning
- **Power BI** — Interactive dashboard and business analytics
- **DAX** — Credit-risk and financial metrics

---

# 🔹 1. Data Preparation & Feature Engineering

The dataset was cleaned and prepared using Python.

### Data Preprocessing

- Handled missing numerical values using median imputation
- Identified numerical and categorical features
- Applied `StandardScaler` for numerical features
- Encoded categorical variables using `OneHotEncoder`

### Feature Engineering

Created additional credit-risk features including:

- **Loan-to-Income Ratio**
- **Employment Category**
- **Age Band**
- **Income Band**
- **Interest Rate Band**

---

# 🔹 2. Machine Learning

Three classification models were evaluated:

- Logistic Regression
- Random Forest
- XGBoost

### Hyperparameter Tuning

`RandomizedSearchCV` was used for hyperparameter tuning with cross-validation.

### Model Evaluation

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Classification Report

Particular attention was given to **Class 1 (loan defaults)** because identifying potential defaults is important in credit-risk analysis.

### Final Model

**XGBoost** was selected for generating the final predictions.

The selected model achieved approximately:

- **94% Accuracy**
- **72% Recall for Default Class**
- **0.83 F1-score for Default Class**

---

# 🔹 3. Credit Risk Prediction

The final XGBoost model generates:

- **Default Probability** — estimated probability of loan default
- **Predicted Default** — binary default prediction
- **Risk Category** — Low, Medium, or High Risk based on predicted probability

These model outputs were exported for further analysis in Power BI.

---

# 🔹 4. Power BI Dashboard

The machine-learning output was imported into Power BI to build an interactive credit-risk analytics dashboard.

### Dashboard Pages

**Executive Overview**
- Total Applicants
- Total Loan Amount
- Default Rate
- Predicted Defaults
- Expected Loss
- Loan Amount at Risk
- Risk Category Distribution

**Loan Portfolio Analysis**
- Loan Intent
- Loan Grade
- Loan Amount
- Interest Rate
- Loan-to-Income Ratio
- Income Bands

**Credit Risk Analysis**
- Default Rate by Loan Grade
- Interest Rate Band
- Employment Category
- Income Band
- Age Band
- Home Ownership

**Model Prediction & Risk**
- Predicted Defaults
- Default Probability
- Risk Categories
- Actual vs Predicted Defaults
- Risk across loan characteristics

# 🔹 5. Key Insights

The analysis explores how credit risk varies across:

- Income levels
- Loan grades
- Interest rates
- Employment categories
- Age groups
- Home ownership
- Loan-to-income ratio
- Loan intent

The project demonstrates how **Machine Learning predictions can be combined with Power BI analytics** to transform credit-risk data into actionable business insights.

