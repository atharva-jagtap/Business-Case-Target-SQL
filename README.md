# 📊 Target Brazil E-Commerce Data Analysis (2016–2018)

## 📌 Project Overview
Target is a globally renowned retail brand known for delivering outstanding value, innovation, and exceptional guest experiences.  
This project focuses on analyzing **Target’s e-commerce operations in Brazil**, using ~100,000 orders placed between **2016 and 2018**.

The goal is to extract **actionable business insights** related to customer behavior, order trends, logistics efficiency, payments, and revenue movement using SQL-based analytics.

---

## 🗂 Dataset Information

- **Time Period:** September 2016 – October 2018  
- **Region:** Brazil  
- **Total Records:** ~100,000 orders  
- **Format:** CSV files  

### 📁 Dataset Files
| File Name | Description |
|---------|------------|
| customers.csv | Customer demographics and location |
| sellers.csv | Seller location details |
| orders.csv | Order status and lifecycle timestamps |
| order_items.csv | Product-level price and freight details |
| payments.csv | Payment methods, installments, and values |
| reviews.csv | Customer ratings and reviews |
| products.csv | Product attributes and dimensions |
| geolocation.csv | Zip-code level latitude & longitude |

---

## 🔍 Analysis Performed

### 1️⃣ Exploratory Data Analysis
- Verified data types for all columns
- Identified order date range
- Counted distinct customer cities and states
- Observed strong customer concentration in **São Paulo (SP)**

---

### 2️⃣ Order Trends & Seasonality
- 📈 **Consistent growth** in orders from 2016 to 2018
- 📅 **Monthly seasonality identified**:
  - Peak orders in **November**
  - Lowest orders in **September**
- ⏰ **Time-of-day behavior**:
  - Most orders placed in the **Afternoon (13–18 hrs)**
  - Least activity during **Dawn (0–6 hrs)**

---

### 3️⃣ Geographic Analysis (Brazil)
- Month-on-month order growth analyzed by state
- **São Paulo (SP)** dominates order volume and revenue
- Northern states show lower penetration and higher logistics cost

---

### 4️⃣ Economic Impact & Revenue Analysis
- 💰 **136.98% increase** in order value from **2017 → 2018** (Jan–Aug)
- Used `payment_value` to measure money flow
- Calculated:
  - Total & Average **order price** per state
  - Total & Average **freight cost** per state
- High freight costs observed in remote states (e.g., Roraima)

---

### 5️⃣ Delivery & Logistics Performance
- Calculated:
  - **Delivery Time:**  
    `order_delivered_customer_date - order_purchase_timestamp`
  - **Delivery Deviation:**  
    `order_delivered_customer_date - order_estimated_delivery_date`
- Identified:
  - Top 5 states with **fastest deliveries**
  - Top 5 states with **slowest deliveries**
  - States consistently delivering **earlier than estimated**
- Southern and urban states perform best in delivery efficiency

---

### 6️⃣ Payment Behavior Analysis
- Month-on-month order volume by payment type
- Credit Card & UPI dominate transactions
- Majority of customers prefer **1–3 installments**
- Very limited usage of high-installment payments

---

## 📈 Key Business Insights
- São Paulo is the **economic and operational backbone**
- Logistics cost optimization needed for remote regions
- Afternoon is the **highest conversion window**
- November is the **critical sales month**
- Faster deliveries correlate strongly with higher satisfaction

---

## 🧠 Business Recommendations
- Optimize freight pricing and logistics routes for high-cost states
- Strengthen delivery infrastructure in North Brazil
- Run targeted **Afternoon flash sales**
- Promote low-EMI options (1–3 installments)
- Prepare inventory & marketing push for **Q4 peak season**

---

## 🛠 Tech Stack
- **SQL (BigQuery)**
- CTEs & Window Functions
- Date & Time Analysis
- Aggregations & Joins

---

## 🔗 Links & Resources

- 📂 **Dataset (Google Drive)**  
  https://drive.google.com/drive/folders/1TGEc66YKbD443nslRi1bWgVd238gJCnb  

- 📄 **Business Case & SQL Queries (PDF)**  
  Target SQL Business Case – Detailed queries, outputs & insights

- 💻 **Tools Used**
  - Google BigQuery
  - SQL Analytics

---

## 👤 Author
**Atharva Jagtap**  
Aspiring Data Analyst / Data Scientist  
Focus Areas: SQL, E-commerce Analytics, Business Insights  

---

## ⭐ How to Use This Project
1. Load CSV files into BigQuery
2. Execute SQL queries provided in the analysis
3. Review insights for business decision-making
4. Extend analysis with dashboards or predictive modeling

---

## 📌 Notes
This project is designed for:
- Data Analyst interviews
- SQL case study discussions
- E-commerce analytics portfolios

---

⭐ *If you found this project useful, feel free to star the repository!*
