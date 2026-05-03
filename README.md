# 🛒 E-commerce Sales Dashboard Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-red?logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

> **Complete E-commerce Sales Analytics with RFM Segmentation, K-Means Clustering & Revenue Forecasting — No dataset download required!**

---

## 📌 Project Overview

This project performs a **full end-to-end sales analytics dashboard** on a simulated e-commerce dataset of **20,000 orders** across **2 years**, **10 Indian cities**, and **6 product categories**.

It covers everything from basic KPIs and trend analysis to advanced customer segmentation using **RFM Analysis** and **K-Means Clustering**, along with **8-week revenue forecasting** using moving averages.

The dataset is **auto-generated inside the notebook** — no Kaggle account or external downloads needed.

---

## 🗂️ Dataset Overview

| Property | Details |
|----------|---------|
| Total Orders | 20,000 |
| Unique Customers | 1,000 |
| Time Period | Jan 2023 – Dec 2024 (2 Years) |
| Cities | 10 Major Indian Cities |
| Categories | 6 Product Categories |
| Products | 35+ Products |
| Features | 14 Columns |

### 📦 Features Description

| Feature | Type | Description |
|---------|------|-------------|
| `order_id` | String | Unique order identifier |
| `order_date` | DateTime | Date of order placement |
| `customer_id` | String | Unique customer identifier |
| `city` | Categorical | City of the customer |
| `category` | Categorical | Product category |
| `product` | Categorical | Product name |
| `quantity` | Numeric | Units ordered |
| `unit_price` | Numeric | Price per unit (₹) |
| `discount_pct` | Numeric | Discount applied (%) |
| `revenue` | Numeric | Final revenue after discount (₹) |
| `profit` | Numeric | Profit earned (₹) |
| `payment_method` | Categorical | UPI / Card / COD / Net Banking |
| `ship_mode` | Categorical | Standard / Express / Same Day |
| `status` | Categorical | Delivered / Returned / Cancelled / Pending |

---

## 🌆 Cities & Categories Covered

**Cities:** Mumbai · Delhi · Bangalore · Hyderabad · Chennai · Pune · Kolkata · Ahmedabad · Jaipur · Lucknow

**Categories:**

| Category | Price Range | Order Share |
|----------|------------|-------------|
| Fashion | ₹299 – ₹5,000 | 28% |
| Electronics | ₹3,000 – ₹80,000 | 20% |
| Home & Kitchen | ₹199 – ₹12,000 | 18% |
| Beauty | ₹99 – ₹3,000 | 12% |
| Sports | ₹299 – ₹8,000 | 12% |
| Books | ₹99 – ₹999 | 10% |

---

## 📂 Project Structure

```
Ecommerce-Sales-Dashboard/
│
├── Ecommerce_Sales_Dashboard.ipynb   ← Main Jupyter Notebook
├── README.md                         ← Project documentation
│
└── images/                           ← Saved plots (after running notebook)
    ├── monthly_trend.png
    ├── quarterly_dow.png
    ├── category_analysis.png
    ├── top_products.png
    ├── city_analysis.png
    ├── payment_shipping.png
    ├── discount_analysis.png
    ├── rfm_segments.png
    ├── kmeans_clusters.png
    ├── revenue_forecast.png
    └── correlation_heatmap.png
```

---

## 📊 Notebook Walkthrough

| Step | Section | Description |
|------|---------|-------------|
| 1 | Install & Import Libraries | All dependencies |
| 2 | Generate Dataset | 20,000 synthetic orders |
| 3 | Data Overview | Info, stats, missing values |
| 4 | Key Business KPIs | Revenue, Profit, AOV, Return Rate |
| 5 | Monthly Sales Trend | Revenue & order count over time |
| 6 | Quarterly & Day-of-Week | Seasonal patterns |
| 7 | Category Analysis | Revenue, share & margin by category |
| 8 | Top Products | Top 15 by revenue & units sold |
| 9 | City-wise Sales | Revenue & order share by city |
| 10 | Payment & Shipping | Method, mode & order status |
| 11 | Discount Impact | Discount vs orders, revenue & profit |
| 12 | RFM Analysis | Customer scoring & segmentation |
| 13 | K-Means Clustering | Elbow method + customer clusters |
| 14 | Revenue Forecasting | 8-week MA forecast with confidence band |
| 15 | Correlation Heatmap | Feature relationships |
| 16 | Final Summary | Complete dashboard KPI summary |

---

## 👥 RFM Customer Segments

| Segment | Description | Strategy |
|---------|------------|---------|
| 🏆 Champions | Bought recently, buy often, spend most | Reward & upsell |
| 💙 Loyal Customers | Buy regularly, good spenders | Loyalty programs |
| 🌱 Potential Loyalists | Recent buyers, moderate frequency | Nurture with offers |
| ⚠️ At Risk | Used to buy but gone quiet | Re-engagement campaigns |
| 😴 Lost | Low recency, frequency & monetary | Win-back campaigns |

---

## 🔵 K-Means Clustering

Uses **K=4 clusters** (chosen via Elbow Method) on scaled RFM features:

| Cluster | Label | Characteristics |
|---------|-------|----------------|
| 0 | High Value | High spend, frequent buyers |
| 1 | Medium Value | Moderate spend & frequency |
| 2 | Low Value | Low spend, infrequent buyers |
| 3 | New / Inactive | Very recent or long inactive |

---

## 🚀 How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/Snehal-Shinde05/Ecommerce-Sales-Dashboard.git
cd Ecommerce-Sales-Dashboard
```

### 2. Install Dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn plotly
```

### 3. Launch Jupyter Notebook
```bash
jupyter notebook Ecommerce_Sales_Dashboard.ipynb
```

### 4. Run All Cells
Go to **Kernel → Restart & Run All**

> ✅ No internet connection needed — dataset generates automatically!

---

## 📦 Requirements

```
python >= 3.8
pandas
numpy
matplotlib
seaborn
scikit-learn
plotly
jupyter
```

Install all at once:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn plotly jupyter
```

---

## 🔑 Key Business Insights

- 🎉 **Festival Season Spike** — Oct to Dec shows ~60% higher revenue than other months
- 🏙️ **Mumbai & Delhi** together contribute ~34% of total revenue
- 👗 **Fashion** is the most ordered category; **Electronics** drives the highest revenue per order
- 💳 **UPI** is the most preferred payment method (~30% of orders)
- 🎯 **Discounts above 20%** reduce profit margins significantly without proportional order increase
- 👑 **Champions** (RFM top segment) generate 3x more revenue than average customers

---

## 🤝 Connect

**GitHub:** [Snehal-Shinde05](https://github.com/Snehal-Shinde05)

---

> ⭐ If you found this project helpful, please give it a star!
