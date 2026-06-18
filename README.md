#  Telecom Customer Churn Prediction & Retention Strategy
**GCI World 2026 - Final Project**

## 📌 Project Overview
This repository contains the final project for the **GCI World 2026** certification. The objective of this project is to act as an IT Consultant to solve a critical business problem for a telecommunications company (Company A): **Customer Churn**. 

Instead of presenting just a machine learning model, this project translates data into a **quantified business proposal**, demonstrating how proactive, AI-driven retention strategies can save the company millions of dollars.

## 🧰 Tech Stack
* **Language:** Python
* **Data Manipulation:** `pandas`, `numpy`
* **Machine Learning:** `scikit-learn`, `xgboost` (XGBClassifier)
* **Data Visualization:** `matplotlib`, `seaborn`

## 📊 Business Problem & Hypothesis
In the telecom industry, acquiring a new customer is significantly more expensive than retaining an existing one. Company A provided a dataset of approximately 100,000 records and ~100 variables. 
* **The Goal:** Predict the likelihood of a customer leaving within the critical 31-60 day window.
* **The Hypothesis:** Customer usage patterns—such as network issues, equipment age, and overage charges—act as early warning signs of dissatisfaction.

## 🧠 Machine Learning Approach
To process over 100 customer variables simultaneously, an **XGBoost Classifier** was trained to output a personalized "Churn Risk Score" for every user. 

* **Evaluation Metric:** ROC-AUC
* **Model Performance:** AUC = 0.6891

### Key Churn Drivers (Feature Importance)
The model successfully identified the root causes of customer churn. The top variables influencing a customer's decision to leave include:
1. `eqpdays` (Equipment Age / Hardware obsolescence)
2. `mou_Mean` (Mean monthly minutes of use)
3. `change_mou` (Recent drops in usage)

## 💰 Quantified Business Impact (ROI)
A predictive model is only valuable if it generates actionable business decisions. A financial simulation was conducted to determine the optimal retention strategy based on the model's predictions.

**Simulation Assumptions:**
* Intervention Cost: $10 per targeted customer.
* Campaign Success Rate: 30%.
* Value Retained: 12 months of customer revenue (L
