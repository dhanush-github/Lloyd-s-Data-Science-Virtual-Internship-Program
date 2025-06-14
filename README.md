# 🔍 Customer Churn Prediction – SmartBank Case Study

This repository showcases an end-to-end data science project for predicting customer churn at **SmartBank**. It includes data preprocessing, EDA, model development, evaluation metrics, and business recommendations to help stakeholders act on insights.

---

## 📁 Project Structure

📦customer-churn-prediction/
├── 📊 Customer_Churn_Data_Large.xlsx # Raw data with 5 sheets

├── 📓 Customer_Churn_Modeling.ipynb # Jupyter notebook with full pipeline

├── 📄 Customer_Churn_Model_Report.pdf # Model training & results summary

├── 📄 Customer_Churn_Model_Report.docx # Same as PDF in Word format

├── 📄 Customer_Churn_EDA_Complete_Report.pdf # EDA, data selection & preprocessing report

├── 📄 Customer_Churn_EDA_Plots_With_Explanation.pdf # Plots with business interpretations

└── 📜 requirements.txt # List of dependencies


---

## 🎯 Objective

Build a reliable and interpretable machine learning model to predict which customers are likely to churn, enabling SmartBank to proactively take retention actions.

---

## 📊 Data Sources (Excel)

- `Customer_Demographics` – Age, Gender, IncomeLevel, etc.
- `Transaction_History` – Purchase behavior (date, amount, category)
- `Customer_Service` – Complaint resolution & interaction details
- `Online_Activity` – Login frequency, last activity, platform usage
- `Churn_Status` – Target label (1 = churned, 0 = retained)

---

## 🔎 Key EDA Insights

- Churned users typically:
  - Log in less frequently
  - Spend less money
  - Have fewer or unresolved customer service interactions
- Income level and platform usage also show slight predictive trends
- Strong class imbalance (~20% churned) handled using `class_weight` and `scale_pos_weight`

---

## 🛠️ Machine Learning Models

| Model               | F1 Score | ROC-AUC | Notes                        |
|--------------------|----------|---------|------------------------------|
| Logistic Regression| ~0.52    | ~0.76   | Interpretable baseline model |
| Random Forest      | ~0.62    | ~0.84   | Robust, feature importance   |
| XGBoost            | ~0.65    | ~0.87   | Best performance overall     |

Evaluation Metrics:
- `F1 Score` for imbalanced class performance
- `ROC-AUC` for classification threshold independence
- `Confusion Matrix` to understand error types

---

## 💡 Business Recommendations

SmartBank can use this model to:
- Flag high-risk customers for retention campaigns
- Use top features (Login Frequency, Amount Spent, etc.) to segment customers
- Deploy churn probabilities in CRM tools
- Reassess churn indicators quarterly via SHAP or retraining

---


---

## 🎯 Objective

Build a reliable and interpretable machine learning model to predict which customers are likely to churn, enabling SmartBank to proactively take retention actions.

---

## 📊 Data Sources (Excel)

- `Customer_Demographics` – Age, Gender, IncomeLevel, etc.
- `Transaction_History` – Purchase behavior (date, amount, category)
- `Customer_Service` – Complaint resolution & interaction details
- `Online_Activity` – Login frequency, last activity, platform usage
- `Churn_Status` – Target label (1 = churned, 0 = retained)

---

## 🔎 Key EDA Insights

- Churned users typically:
  - Log in less frequently
  - Spend less money
  - Have fewer or unresolved customer service interactions
- Income level and platform usage also show slight predictive trends
- Strong class imbalance (~20% churned) handled using `class_weight` and `scale_pos_weight`

---

## 🛠️ Machine Learning Models

| Model               | F1 Score | ROC-AUC | Notes                        |
|--------------------|----------|---------|------------------------------|
| Logistic Regression| ~0.52    | ~0.76   | Interpretable baseline model |
| Random Forest      | ~0.62    | ~0.84   | Robust, feature importance   |
| XGBoost            | ~0.65    | ~0.87   | Best performance overall     |

Evaluation Metrics:
- `F1 Score` for imbalanced class performance
- `ROC-AUC` for classification threshold independence
- `Confusion Matrix` to understand error types

---

## 💡 Business Recommendations

SmartBank can use this model to:
- Flag high-risk customers for retention campaigns
- Use top features (Login Frequency, Amount Spent, etc.) to segment customers
- Deploy churn probabilities in CRM tools
- Reassess churn indicators quarterly via SHAP or retraining

---

