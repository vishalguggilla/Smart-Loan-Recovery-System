# 💰 Smart Loan Recovery System

The **Smart Loan Recovery System** is a machine learning project that predicts the likelihood of loan recovery based on borrower data.  
It helps financial institutions identify **high-risk customers**, visualize repayment patterns, and make **data-driven recovery decisions**.

---

## 📊 Project Overview

The project involves:
- Exploratory Data Analysis (EDA) to understand loan and income distributions
- Visualization using **Plotly** for interactive analysis
- Machine Learning model training for predicting loan recovery probability
- Evaluation of model performance using standard metrics

---

## ⚙️ Tech Stack

- **Language:** Python  
- **Libraries Used:**
  - pandas
  - numpy
  - scikit-learn
  - plotly
  - matplotlib / seaborn (optional)
  - joblib (for model saving)

---

## 🧠 Machine Learning Workflow

### 1️⃣ Data Preprocessing
- Load dataset (`loan-recovery.csv`)
- Handle missing values
- Encode categorical variables
- Normalize numerical data

### 2️⃣ Exploratory Data Analysis
Interactive visualizations using Plotly:
- Loan amount distribution  
- Relationship between **loan amount** and **monthly income**
- Correlation between recovery rate and borrower profile

### 3️⃣ Model Building
- Train supervised ML models like:
  - Logistic Regression  
  - Random Forest  
  - XGBoost (optional)
- Split data into train/test sets
- Compare accuracy, precision, recall, F1-score

### 4️⃣ Evaluation
Metrics used:
- Accuracy
- Confusion Matrix
- ROC-AUC Curve
- Precision-Recall Analysis

---

## 📈 Sample Visualization

Example of loan amount distribution visualization using Plotly:

```python
fig = px.histogram(df, x='Loan_Amount', nbins=30, marginal="violin", opacity=0.7,
                   title="Loan Amount Distribution & Relationship with Monthly Income",
                   labels={'Loan_Amount': "Loan Amount ($)", 'Monthly_Income': "Monthly Income"},
                   color_discrete_sequence=["royalblue"])
