# 💳 Credit Card Default Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Classification-green)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)
![License](https://img.shields.io/badge/License-Academic-lightgrey)

## 📌 Overview

Credit default prediction is a critical problem in financial risk management. Banks and financial institutions need reliable models to identify customers who may fail to repay credit in order to reduce financial losses.

This project develops a **machine learning pipeline to predict credit card default risk** using customer demographic information, billing behavior, and payment history.

The workflow includes:

* Data preprocessing
* Exploratory Data Analysis (EDA)
* Feature engineering
* Handling class imbalance using **SMOTE**
* Training multiple machine learning models
* Model evaluation and comparison
* Selection of the best-performing model

The **Random Forest classifier** achieved the best overall performance.

---

## 🎯 Problem Statement

The objective is to build a predictive model that can classify whether a customer will **default on their credit card payment in the upcoming month** based on their historical financial behavior and demographic attributes.

This helps financial institutions:

* Detect high-risk customers early
* Reduce credit losses
* Improve credit approval decisions
* Maintain a balanced risk strategy

---

## ⚙️ Project Workflow

```
Data Collection
      ↓
Data Preprocessing
      ↓
Exploratory Data Analysis
      ↓
Feature Engineering
      ↓
Handling Class Imbalance (SMOTE)
      ↓
Model Training
      ↓
Model Evaluation
      ↓
Best Model Selection
```

---

## 📊 Exploratory Data Analysis

EDA was performed to understand customer behavior and financial patterns.

Key variables analyzed:

* Credit limit
* Age distribution
* Payment history
* Billing amounts
* Repayment amounts
* Education and marital status

### Key Insights

* Payment delays strongly correlate with default probability
* Higher credit utilization indicates higher risk
* Irregular repayment patterns signal financial distress
* Younger customers show slightly higher default rates

---

## 🧠 Feature Engineering

Several derived features were created to improve model performance:

| Feature               | Description                          |
| --------------------- | ------------------------------------ |
| Utilization Ratio     | Average bill amount / credit limit   |
| Payment-to-Bill Ratio | Repayment relative to billing        |
| Delinquency Streak    | Longest sequence of delayed payments |
| Avg Monthly Bill      | Average billing amount               |
| Monthly Payment Ratio | Payment behavior over time           |

These features capture **financial behavior patterns more effectively than raw data**.

---

## 🤖 Machine Learning Models Used

The following classification algorithms were trained and evaluated:

* Logistic Regression
* Random Forest
* XGBoost
* AdaBoost
* CatBoost
* LightGBM
* K-Nearest Neighbors
* Support Vector Classifier

---

## 📈 Model Evaluation

Models were evaluated using multiple performance metrics:

* Accuracy
* Precision
* Recall
* F1 Score
* **F2 Score**
* ROC-AUC

The **F2 Score** was emphasized because it prioritizes **recall**, which is important in credit risk modeling to avoid missing true defaulters.

---

## 🏆 Final Model Performance

The **Random Forest classifier** achieved the best results.

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 0.9061 |
| Precision | 0.9339 |
| Recall    | 0.8740 |
| F2 Score  | 0.8854 |
| ROC-AUC   | 0.9595 |

---

## 💼 Business Impact

The model can assist financial institutions in:

* Identifying high-risk customers
* Improving credit scoring systems
* Reducing financial losses
* Optimizing loan approval strategies

A classification **threshold of 0.5** was selected to balance false positives and false negatives.

---

## 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* XGBoost
* LightGBM
* CatBoost
* Imbalanced-Learn (SMOTE)

---

## 📁 Project Structure

```
credit-default-prediction/

│
├── data/
│   ├── train_dataset.csv
│   └── validation_dataset.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── models/
│   └── random_forest_model.pkl
│
├── report/
│   └── project_report.pdf
│
└── README.md
```

---

