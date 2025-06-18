# Taxi
# 🕵️‍♂️ Fraud Detection Analysis – ML & Exploratory Data Project

This repository contains a structured data science pipeline for detecting and analyzing fraud in ride-based transactions. It combines exploratory data analysis, clustering, and machine learning to identify risky behaviors and propose actionable product decisions.

---

## 📁 Project Structure

| Notebook | Description |
|----------|-------------|
| `0.1 — Data import and descriptive analysis.ipynb` | Data loading, cleaning, and initial descriptive statistics |
| `02_Correlation_cleaned.ipynb` | Correlation analysis to identify key relationships between variables |
| `0.3 Geographic Visualization.ipynb` | Country-level visualization of risk patterns and transaction breakdowns |
| `0.4 — Regression.ipynb` | Regression analysis for price-based behavior and prediction signals |
| `0.5 — Clustering.ipynb` | User behavior clustering to isolate patterns among fraud-prone users |
| `structured_fraud_analysis_notebook.ipynb` | Combined insights and ML model building with feature importance and evaluation |

---

## 🎯 Project Goals

- Detect patterns leading to **first-time failed payments**
- Segment users by behavior to improve fraud detection
- Build a predictive model to classify failed vs. successful payments
- Evaluate model using classification metrics and ROC AUC
- Visualize geographic and behavioral signals of fraud

---

## 📊 Key Results

- ✅ **Model Accuracy**: 97%  
- 🧠 **ROC AUC Score**: 0.94  
- 🔑 **Top Predictors**: `log_price_per_km`, `price`, `failed_before_success`, `is_first_attempt`  
- 🌍 **Insights**: High failure rates in specific country–device clusters

---

## 🚀 Product Recommendations

- Require **pre-ride card verification** for high-risk segments
- Apply **soft blocks** (email/phone verification) to suspicious first-time users
- Cap ride prices for **unverified or risky users**

---

## 📈 Interactive Tableau Dashboard

▶️ View the full visual story here:  
🔗 [Tableau Storyboard – Final Results](https://public.tableau.com/app/profile/hlib.havryliuk/viz/finalstoryboard12/Story1?publish=yes)

---

## 🧰 How to Use

1. Clone this repository  
2. Open notebooks in Jupyter or VSCode  
3. Follow the project pipeline from data import to modeling  
4. Explore final analysis in Tableau via the link above
