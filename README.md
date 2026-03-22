# DevelopersHub Corporation — Data Science & Analytics Internship

**Intern:** Muhammad Yahya Imran  
**Program:** Data Science & Analytics Internship  
**Organization:** DevelopersHub Corporation  

---

## Overview

This repository presents all 5 tasks undertaken during the Data Science & Analytics Internship at DevelopersHub Corporation. Each task is built around a real-world dataset and covers the full pipeline — from raw data handling and exploratory analysis to machine learning model development and performance evaluation.

**Tools & Libraries:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, KaggleHub

---

## Task 1: Exploring and Visualizing a Simple Dataset

**Objective:**
Get hands-on experience reading, summarizing, and visualizing data using the classic Iris dataset.

**Approach:**
- Imported the Iris dataset via the Seaborn library
- Inspected the data structure using `.shape`, `.info()`, and `.describe()`
- Generated scatter plots, histograms, box plots, and a correlation heatmap for visual exploration
- Built a Random Forest Classifier to assess how well the features separate species

**Key Findings:**
- The dataset is evenly distributed with exactly 50 records per species and zero missing values
- Petal length and petal width proved to be the most discriminative features
- The Setosa species is distinctly separable from Versicolor and Virginica
- The Random Forest model delivered strong classification performance on this dataset

---

## Task 2: Credit Risk Prediction

**Objective:**
Determine whether a loan applicant is at risk of defaulting on their loan.

**Dataset:** Loan Prediction Dataset (Kaggle)

**Approach:**
- Filled missing values using mode for categorical columns and median for numerical ones
- Plotted distributions of loan amounts, applicant income, and approval outcomes
- Developed Logistic Regression and Decision Tree models for binary classification
- Assessed model performance via accuracy scores and confusion matrices

**Key Findings:**
- An applicant's credit history turned out to be the dominant predictor for loan approval
- Graduate applicants had a noticeably higher rate of loan approvals compared to non-graduates
- Higher-income applicants were associated with larger sanctioned loan amounts
- Logistic Regression showed stable and reliable performance across evaluations

---

## Task 3: Customer Churn Prediction (Bank Customers)

**Objective:**
Predict which bank customers are at risk of discontinuing their services.

**Dataset:** Churn Modelling Dataset (Kaggle)

**Approach:**
- Removed non-informative columns such as RowNumber, CustomerId, and Surname
- Used Label Encoding for Gender and One-Hot Encoding for the Geography column
- Trained and compared Logistic Regression and Random Forest classifiers
- Examined feature importance scores to pinpoint the main drivers of churn

**Key Findings:**
- Roughly 20% of customers in the dataset had churned
- Age emerged as the strongest churn predictor — older customers are more likely to exit
- German customers exhibited a disproportionately higher churn rate compared to other regions
- Customers holding higher balances but subscribed to fewer products showed elevated churn risk
- Random Forest outperformed Logistic Regression, likely due to non-linear relationships in the data

---

## Task 4: Predicting Insurance Claim Amounts

**Objective:**
Forecast the medical insurance charges incurred by individuals based on demographic and lifestyle data.

**Dataset:** Medical Cost Personal Dataset (Kaggle)

**Approach:**
- Converted categorical variables (sex, smoker status, region) to numeric form via Label Encoding
- Explored how BMI, age, and smoking habits correlate with insurance charges through visualizations
- Fitted both a Linear Regression model and a Random Forest Regressor
- Compared models using MAE, RMSE, and R² Score metrics

**Key Findings:**
- Smoking status had the most significant effect on charges — smokers face substantially higher costs
- Both age and BMI show a consistent positive correlation with insurance expenses
- The combination of obesity (BMI > 30) and smoking resulted in the highest observed charges
- Geographic region and biological sex had minimal influence on the predicted amounts
- The Random Forest Regressor yielded a superior R² score and reduced prediction error versus Linear Regression

---

## Task 5: Personal Loan Acceptance Prediction

**Objective:**
Identify which customers are most likely to respond positively to a personal loan offer.

**Dataset:** Bank Marketing Dataset — UCI Machine Learning Repository (Kaggle)

**Approach:**
- Conducted exploratory analysis on demographic features such as age, occupation, marital status, and education level
- Encoded all categorical variables numerically using Label Encoding
- Trained Logistic Regression and Decision Tree classifiers on the processed data
- Reviewed feature importance to highlight the customer segments most receptive to loan offers

**Key Findings:**
- The dataset is class-imbalanced — the majority of customers declined the loan offer
- Students and retired individuals demonstrated comparatively higher acceptance rates
- Customers reached through cellular contact were more responsive than those contacted by telephone
- The duration of the last call and the count of prior contacts were the strongest predictors
- Logistic Regression performed competitively, benefiting from the data's largely linear decision boundary

---

## Repository Structure

```
DevelopersHub-Internship/
├── Task1_Iris_EDA.ipynb
├── Task2_Credit_Risk_Prediction.ipynb
├── Task3_Customer_Churn_Prediction.ipynb
├── Task4_Insurance_Claims_Prediction.ipynb
├── Task5_Loan_Acceptance_Prediction.ipynb
└── README.md
```

---

## How to Run

1. Open any notebook in Google Colab or Jupyter Notebook
2. Install the required library if it isn't already present:
   ```
   pip install kagglehub
   ```
3. Execute all cells sequentially from top to bottom
4. Datasets are fetched automatically — via `kagglehub` for Tasks 2–5 and via `seaborn` for Task 1

---

*Submitted as part of the DevelopersHub Corporation Data Science & Analytics Internship Program.*
