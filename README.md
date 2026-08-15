# 🛒 E-Commerce Fraud Detection & Customer Analytics

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-3776AB)

An exploratory data analysis (EDA) and feature engineering project aimed at identifying fraudulent transaction patterns and customer behavioral traits in an e-commerce platform dataset.

---

## 📌 Executive Summary

Initial univariate and bivariate analyses revealed that individual customer attributes (such as `loyalty_score`, `churn_risk`, and `days_since_last_purchase`) exhibit near-100% distribution overlap between legitimate and fraudulent shoppers. 

However, multi-variable interactions—specifically **Country** paired with **Preferred Category**—revealed localized high-risk fraud hotspots.

---

## 📊 Key Findings & Insights

* **Univariate Weak Predictors:** Individual metrics (e.g., `loyalty_score` and `churn_risk`) show statistically insignificant correlations ($\vert{}r\vert{} < 0.012$) with fraud. Fraudulent profiles closely mirror normal customer behaviors.
* **Geographic & Category Hotspots:**
  * **USA + Home Category:** Highest risk segment with a **10% fraud rate**.
  * **Japan + Electronics:** Secondary hotspot with a **9% fraud rate**.
  * **Zero-Fraud Segments:** Combinations like `USA + Beauty` and `China + Sports` showed **0% fraud**.
* **Feature Engineering:** Order-density ratios (e.g., $\frac{\text{loyalty\_score}}{\text{total\_orders}}$) confirmed that standalone aggregations in this dataset do not linearly separate fraud without higher-order interaction features.

---

## 🛠️ Tech Stack & Libraries

* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Seaborn, Matplotlib

---

## 🚀 How to Run the Notebook

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Your-Username/Your-Repo-Name.git](https://github.com/Your-Username/Your-Repo-Name.git)
   cd Your-Repo-Name
