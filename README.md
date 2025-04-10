# 🧠 Customer Segmentation Using RFM Analysis and K-Means Clustering


This project showcases how to use **RFM (Recency, Frequency, Monetary) analysis** and **unsupervised machine learning** to identify meaningful customer segments—helping businesses target the right people with the right message at the right time. Helpful for **data-driven marketing strategy** project where raw sales data meets analytical thinking.


---

## 💡 Why This Project?

In today’s competitive landscape, **knowing your customer is everything**. Generic marketing is costly and ineffective. That’s where segmentation comes in. With proper segmentation, businesses can:

- Improve retention by rewarding loyalty
- Reduce churn through proactive engagement
- Boost sales via personalized offers
- Optimize marketing spend

Using **RFM analysis**, and **K-Means clustering**, this project walks through a full customer segmentation pipeline—from raw CSV to actionable insights.

---

## 🧭 Project Overview

| Stage | Description |
|-------|-------------|
| **Data Preparation** | Cleaned and explored the dataset (duplicates, missing values, types) |
| **EDA & Visualization** | Explored sales trends, outliers, and skewness across time and categories |
| **RFM Calculation** | Engineered features: Recency, Frequency, Monetary |
| **RFM Scoring** | Scaled values using quantile binning to prepare for clustering |
| **Clustering** | Applied K-Means to segment customers and used the Elbow Method for optimization |
| **Interpretation** | Labeled and described clusters with business-friendly insights |
| **Marketing Strategy** | Proposed actionable strategies for each customer group |

---

## 🔍 Business Questions Addressed

- Who are our most valuable customers?
- Which customers are at risk of churning?
- How can we personalize marketing strategies for different customer groups?
- Where should we focus retention or reactivation efforts?

---

## 📊 Exploratory Data Analysis (EDA)

- Identified sales peaks across quarters and years
- Visualized distributions of **Sales**, **Quantity**, **PriceEach**, and more
- Found skewness and outliers—important for clustering accuracy
- Verified no missing values or duplicate records

---

## 🧮 RFM Feature Engineering

**RFM** is a proven technique to quantify customer value:

| Metric     | Meaning                                |
|------------|----------------------------------------|
| Recency    | Days since last purchase (lower = better) |
| Frequency  | Total number of purchases              |
| Monetary   | Total spend by customer                |

---

## 🎯 RFM Scoring Strategy

Customers were scored from **1 to 4** based on percentile ranks:

- **Recency:** Lower values → higher scores  
- **Frequency & Monetary:** Higher values → higher scores  

This made the data ordinal and suitable for K-Means clustering.

---

## 📦 Clustering with K-Means

Used **K-Means clustering** to group customers based on RFM behavior.

- Optimal **K = 4** determined via the **Elbow Method**
- Scaled features were clustered without further standardization
- Final cluster labels were interpreted for real-world meaning

---

## 🧠 Customer Segments Identified

| Cluster | Description | Label |
|--------:|-------------|-------|
| 0 | Long-time customers, moderately frequent, high spend | 🔁 *Departing Loyalists* |
| 1 | Recent, frequent, high-spending customers | 💎 *Best Customers* |
| 2 | Infrequent, low-value, inactive customers | 💤 *Dormant Customers* |
| 3 | New, low-frequency, low-spend customers | 🌱 *New & Unengaged* |

---

## 📣 Suggested Marketing Strategies

### 💎 Best Customers (Active)
- VIP loyalty programs
- Exclusive early access and special rewards
- Personalized thank-you gifts

### 🌱 New & Random Customers
- Welcome offers and onboarding emails
- Targeted product recommendations
- Incentives for second purchase

### 🔁 Former Loyalists (Departing)
- Win-back campaigns
- Personalized "We miss you" discounts
- Feedback surveys to understand drop-off

### 💤 Inactive Customers
- Low-cost reactivation offers
- Consider deprioritizing if unresponsive

---

## 🧰 Tools & Technologies

- **Python**
  - `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
- **Jupyter Notebook**
- **Git & GitHub**
- **Business Understanding** for customer journey and strategy

---

## 📈 Results & Impact

This segmentation enables marketers and business analysts to:

- Focus resources on high-value customers
- Personalize communication for increased engagement
- Recover lost revenue from lapsed customers
- Build data-informed retention strategies

---

## 📄 License

This project is licensed under the MIT License.
