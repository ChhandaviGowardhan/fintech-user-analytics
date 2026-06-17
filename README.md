# 📊 Fintech Product Analytics & User Behaviour Analysis

---

## 🚀 Overview

This project simulates a real-world fintech product analytics workflow by analyzing user onboarding behavior, transaction activity, acquisition performance, retention patterns, **customer segmentation, and campaign effectiveness**.

The objective is to derive meaningful business insights that help improve user conversion, engagement, and long-term retention using Python, SQL, and Power BI.

---

## 💼 Business Problem

Fintech platforms need to answer critical questions such as:

* Which acquisition channels bring the most valuable users?
* Where do users drop off during onboarding?
* How do users behave after their first transaction?
* Are users retained over time?
* Which customer segments contribute most to revenue?
* How effective are marketing campaigns?

This project addresses these questions through structured data analysis and visualization.

---

## 🎯 Objectives

* Analyze onboarding and conversion performance
* Evaluate acquisition channel effectiveness
* Study transaction and revenue trends
* Perform cohort-based retention analysis
* Analyze campaign performance
* Perform customer segmentation (RFM-based)
* Build an interactive Power BI dashboard for decision-making

---

## 🛠️ Tech Stack

| Category        | Tools                     |
| --------------- | ------------------------- |
| Programming     | Python                    |
| Data Processing | Pandas, NumPy             |
| Querying        | SQL (SQLite)              |
| Visualization   | Power BI                  |
| Development     | VS Code, Jupyter Notebook |

---

## 🗂️ Dataset

The dataset was synthetically generated to mimic realistic fintech user behavior.

### 👤 Users Dataset (~5,000 records)

* user_id
* signup_date
* acquisition_channel
* campaign_id
* kyc_completed
* is_converted

---

### 💳 Transactions Dataset (~54,000 records)

* transaction_id
* user_id
* transaction_date
* amount
* transaction_type
* status

---

### 📢 Campaign Dataset (10 campaigns)

* campaign_id
* campaign_name
* channel
* start_date
* end_date
* cost

---

## 📊 Key Metrics

### Product Metrics

* Total Users
* KYC Completion Rate
* Conversion Rate

### Transaction Metrics

* Total Transactions
* Total Revenue
* Average Transaction Value

### Retention Metrics

* Cohort Retention Rate
* User Repeat Behavior

### Acquisition Metrics

* Users by Channel
* Conversion Rate by Channel
* Revenue Contribution by Channel
* Average Revenue per User (ARPU)

### Segmentation Metrics

* RFM Segments (High Value, Loyal, At Risk, Low Value, No Activity)
* Revenue by Segment
* Average Spend by Segment

### Campaign Metrics

* Users per Campaign
* Revenue per Campaign
* Campaign Conversion Trends

---

## 🧠 SQL Analysis

SQL was used to extract key business insights such as:

* Funnel conversion rates
* Transaction summaries
* Acquisition channel performance
* Campaign performance analysis
* Customer segmentation logic
* Retention cohort analysis

Example:

```sql
SELECT 
    acquisition_channel,
    COUNT(DISTINCT user_id) AS users,
    SUM(total_amount) AS revenue
FROM users
GROUP BY acquisition_channel;
```

---

## 📊 Dashboard Overview

The Power BI dashboard is divided into **three analytical pages**.

---

### 🟦 Page 1 — Business Performance Overview

This page provides a high-level view of overall product performance.

**Includes:**

* KPI Cards (Users, KYC, Conversion, Revenue)
* Transaction trends over time
* Revenue growth analysis
* Conversion performance

---

### 🟩 Page 2 — User Behavior & Acquisition Insights

This page focuses on understanding user quality and channel effectiveness.

**Includes:**

* User distribution by acquisition channel
* Conversion rate comparison across channels
* Revenue contribution by channel
* Average revenue per user (ARPU)
* Cohort-based retention heatmap

---

### 🟨 Page 3 — Customer Segmentation & Campaign Analysis

This page focuses on deeper behavioral and marketing insights.

**Includes:**

* User distribution by segment
* Average spend per segment
* Revenue contribution by segment
* Revenue by campaign

---

## 📷 Dashboard Screenshots

### 🔹 Page 1 — Business Performance Overview

![Page 1](images/business_overview.png)

---

### 🔹 Page 2 — User Behavior & Acquisition Insights

![Page 2](images/user_insights.png)

---

### 🔹 Page 3 — Customer Segmentation & Campaign Analysis

![Page 3](images/customer_segmentation.png)

---

## 📈 Key Insights

* 📉 Significant drop-off observed between signup and conversion
* 📣 Referral channels show higher conversion efficiency
* 💰 High-value users contribute disproportionately to total revenue
* ⚠️ Large portion of users fall into "At Risk" category
* 📊 Some campaigns drive high revenue but vary in user acquisition quality
* 🔁 Retention declines over time but stabilizes after initial drop

---

## 📁 Project Structure

```plaintext
fintech-user-analytics/
│
├── data/
│   ├── raw/
│   └── processed/
|   └── fintech.db
│
├── notebooks/
│   ├── data_generation.ipynb
│   └── sql_analysis.ipynb
│
├── powerbi/
│   └── Dashboard.pbix
|   └── Dashboard.pdf
│
├── images/
│   ├── business_overview.png
│   ├── user_insights.png
│   └── customer_segmentation.png
|
├── requirements.txt
│
└── README.md
```

---

## 💡 Conclusion

This project demonstrates an end-to-end product analytics workflow, covering:

* Data generation and preprocessing
* SQL-based business analysis
* Customer segmentation (RFM)
* Campaign performance evaluation
* Dashboard creation for stakeholder insights

It highlights how data can be leveraged to evaluate product performance and drive strategic decisions.

---

## 🔗 Future Improvements

* Advanced segmentation (K-Means clustering)
* Predictive modeling (churn prediction)
* Real-time data pipeline integration
* More accurate campaign ROI modeling

---

## 👩‍💻 Author

**Chhandavi Gowardhan**
Aspiring Data Analyst

Skills: Python • SQL • Power BI • Data Analytics • Product Analytics

---
