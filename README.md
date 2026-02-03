# Customer Churn Prediction & Retention Dashboard

## 📌 Project Overview
This project focuses on predicting customer churn and identifying high-risk customers to support retention strategies in a subscription-based business context.  
Instead of producing only churn labels, the model generates churn probabilities and risk categories, enabling actionable business insights and prioritization.

---

## 🧠 Problem Statement
Customer churn leads to significant revenue loss if not addressed proactively.  
The objective of this project is to:
- Predict the probability of churn for each customer
- Identify high-risk **active** customers
- Provide an actionable retention list through an interactive dashboard

---

## 📂 Dataset
The project uses a customer subscription dataset containing demographic, service usage, billing, and contract-related features.  
The dataset includes historical churn information and is used to learn patterns associated with customer attrition.

---

## 🔧 Tools & Technologies
- **Python:** Pandas, NumPy, Scikit-learn  
- **Machine Learning:** Logistic Regression, Random Forest, XGBoost, LightGBM, CatBoost  
- **Visualization:** Power BI  
- **EDA & Modeling:** Matplotlib, Seaborn  

---

## 📊 Methodology
1. Performed exploratory data analysis to identify key churn drivers such as contract type, tenure, and internet service.
2. Applied feature engineering techniques including ordinal encoding, one-hot encoding, and feature scaling.
3. Trained and evaluated multiple classification models using stratified cross-validation.
4. Selected **Logistic Regression** based on recall and F1-score to prioritize identifying churn-prone customers.
5. Generated churn probabilities and segmented customers into **Low**, **Medium**, and **High** risk categories.
6. Filtered predictions to active customers only to ensure business relevance.
7. Delivered insights through an interactive Power BI dashboard.

---

## 📈 Key Insights
- Month-to-month contract customers exhibit the highest churn risk.
- Fiber optic users show higher churn probability compared to DSL users.
- Churn risk decreases significantly as customer tenure increases.

---

## 📊 Dashboard

### Executive Overview
Provides a high-level view of churn risk distribution and key churn drivers.
![Overview](dashboard/overview_page.png)

### High-Risk Customer Action List
Displays the top high-risk active customers, enabling targeted retention actions.
![Action List](dashboard/action_list_page.png)

---

## 🎯 Business Impact
- Enables retention teams to prioritize customers most likely to churn.
- Supports focused retention campaigns instead of broad, costly interventions.
- Improves decision-making using probability-based risk scoring rather than binary predictions.
