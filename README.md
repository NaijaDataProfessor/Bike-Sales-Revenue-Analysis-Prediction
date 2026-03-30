# 🚴‍♂️ Bike Sales Revenue Analysis & Prediction

## 📌 Project Overview

This project is an **end-to-end data analytics and machine learning workflow** focused on understanding and predicting revenue in a bike sales dataset across Europe and other regions.

The project was executed in three major stages:

1. **Data Analysis with SQL**
2. **Data Visualization with Power BI**
3. **Machine Learning Modeling in Python (Jupyter Notebook)**

The goal was not just to build a predictive model, but to **extract meaningful business insights and translate them into data-driven decisions**.

---

## 🧰 Tools & Technologies

* **SQL (MySQL)** – Data cleaning & exploratory analysis
* **Power BI** – Dashboarding & visualization
* **Python (Pandas, Scikit-learn)** – Machine learning & feature engineering
* **Jupyter Notebook** – Model development

---

## 🗄️ Stage 1: SQL Analysis

### 🔍 Data Preparation

* Removed duplicate records using `SELECT DISTINCT`
* Created a clean working dataset for reliable analysis

---

### 📊 Key Business Metrics

* **Total Transactions:** 112,036
* **Total Revenue:** 84,826,772

---

### 🌍 Revenue by Geography

#### Top Countries by Revenue

* United States → 27.7M
* Australia → 21.2M
* United Kingdom → 10.5M
* Germany → 8.9M
* France → 8.4M
* Canada → 7.9M

#### Top States by Revenue

* California → 17.5M
* England → 10.5M
* New South Wales → 9.1M
* British Columbia → 7.8M

👉 **Insight:** Revenue is highly concentrated in a few key regions.

---

### 🛍️ Product Performance

#### Category Contribution

* Bikes → 61.4M
* Accessories → 15.0M
* Clothing → 8.3M

👉 **Insight:** Bikes dominate revenue, contributing the majority share.

---

#### Most Profitable Products

Top-performing products include:

* Mountain-200 Black
* Road-150 Red
* Sport-100 Helmet

👉 **Insight:** A small number of products drive a large portion of profit (Pareto effect).

---

### 👥 Customer Segmentation

#### Revenue by Age Group

* Adults (35–64) → 42.3M
* Young Adults (25–34) → 30.4M
* Youth (<25) → 11.6M
* Seniors (64+) → Minimal

👉 **Insight:** Core revenue comes from economically active age groups.

---

#### Revenue by Gender

* Male → 43.1M
* Female → 41.6M

👉 **Insight:** Revenue is relatively balanced across gender.

---

### 📈 Time-Based Trends

#### Monthly Trends

* Highest → December (~814 avg revenue)
* Strong months → May, June
* Lowest → October

👉 **Insight:** Clear seasonality with peaks toward year-end.

---

#### Yearly Trends

* Growth from 2011 → 2015
* Peak in 2015 (~19.9M)
* Slight decline in 2016

👉 **Insight:** Business experienced growth followed by stabilization.

---

## 📊 Stage 2: Power BI Visualization

The SQL insights were translated into interactive dashboards to:

* Track revenue performance across regions
* Visualize product and category trends
* Monitor customer segmentation
* Identify seasonal sales patterns

👉 This made insights more accessible for **business stakeholders**.

---

## 🤖 Stage 3: Machine Learning (Revenue Prediction)

### 🎯 Objective

Predict revenue and identify the key drivers influencing sales.

---

### ⚠️ Key Challenge: Data Leakage

Initial models showed near-perfect performance due to:

* Revenue being indirectly computed from features like quantity and cost

This was corrected by removing leakage variables, resulting in a more realistic model.

---

### 📈 Model Performance

* **Best Model:** Xgboost
* **R² Score:** ~0.71
* **MAE:** ~300

👉 The model explains ~71% of revenue variation.

---

### 🧠 Feature Engineering

Engineered features included:

* Price-based metrics (relative pricing, ranking)
* Product-level aggregates
* Time features (month, day of week)
* Interaction features

---

### 🔍 Key ML Insights

* Revenue is driven more by **customer demographics and product categories** than pricing
* Product performance improves when contextualized (frequency, averages)
* Pricing alone is not a strong predictor without context
* Removing leakage is critical for building trustworthy models

---

## 💼 Business Insights

* Revenue is concentrated in specific **countries and states**
* **Bikes** are the primary revenue driver
* A small number of products generate most of the profit
* **Adults (35–64)** are the most valuable customer segment
* Sales show strong **seasonality**, especially toward year-end
* Customer behavior plays a bigger role than pricing alone

---

## 🚀 Conclusion

This project demonstrates a complete data workflow:

* From **raw data cleaning (SQL)**
* To **insight generation (SQL + Power BI)**
* To **predictive modeling (Machine Learning)**

The key takeaway:

> High-performing models are not the goal —
> building models that reflect real business behavior is what truly matters.

---

## 📌 Next Steps

* Improve model performance (target R²: 0.80+)
* Incorporate more behavioral and external data
* Deploy model for real-time prediction use cases

---

## 🔗 Author

Tolulope Emuleomo
Data Analyst | Machine Learning Enthusiast


