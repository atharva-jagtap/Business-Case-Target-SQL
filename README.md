📊 Target Brazil E-Commerce Data Analysis (2016–2018)
📌 Project Overview

Target is a globally renowned retail brand known for delivering exceptional customer experiences. This project analyzes Target’s e-commerce operations in Brazil using ~100,000 orders placed between 2016 and 2018.

The objective is to extract business insights, understand customer behavior, logistics performance, payment trends, and provide actionable recommendations using SQL-based analysis.

🗂 Dataset Description

The dataset consists of 8 CSV files covering customers, orders, payments, products, sellers, logistics, and reviews:

File Name	Description
customers.csv	Customer demographics and location
sellers.csv	Seller details and location
orders.csv	Order lifecycle timestamps and status
order_items.csv	Product-level order and freight details
payments.csv	Payment types, installments, and values
reviews.csv	Customer ratings and feedback
products.csv	Product attributes and dimensions
geolocation.csv	Zip code to latitude/longitude mapping
🔍 Key Analysis Performed
1️⃣ Exploratory Data Analysis

Inspected data types of all columns

Identified order date range: Sep 2016 – Oct 2018

Counted customer cities and states

Observed strong customer concentration in São Paulo (SP)

2️⃣ Order Trends & Seasonality

📈 Orders increased steadily from 2016 → 2018

📅 Seasonality observed:

Highest orders: November

Lowest orders: September

⏰ Preferred order time:

Most orders placed in the Afternoon (13–18 hrs)

Least activity during Dawn (0–6 hrs)

3️⃣ Geographic Insights (Brazil Focus)

Month-on-month order growth analyzed per state

SP (São Paulo) dominates order volume

Less penetration in northern states (e.g., RR – Roraima)

4️⃣ Economic Impact & Revenue Analysis

💰 136.98% increase in total order value from 2017 → 2018 (Jan–Aug)

Used payment_value to measure money flow

Computed:

Total & Average order price per state

Total & Average freight value per state

SP leads in total revenue

RR shows highest average freight cost (logistics challenge)

5️⃣ Delivery & Logistics Performance

Calculated:

time_to_deliver = actual delivery time

diff_estimated_delivery = early/late delivery

Identified:

🚚 Top 5 states with fastest deliveries

⏳ Top 5 states with slowest deliveries

⚡ States consistently delivering earlier than estimated

SP, MG, PR perform well in delivery efficiency

6️⃣ Payment Behavior Analysis

Month-on-month order volume by payment type

Credit cards & UPI dominate transactions

Majority of orders placed with 1–3 installments

Very few zero-installment or high-EMI orders

📈 Key Business Insights

São Paulo is the economic and operational backbone

Logistics costs spike in remote states → optimization opportunity

Afternoon shopping peaks → ideal time for promotions

November sales surge → align inventory & marketing

Faster delivery strongly correlates with higher customer satisfaction

🧠 Recommendations

Optimize freight pricing for high-cost states

Improve logistics in North Brazil regions

Push Afternoon flash sales

Strengthen EMI offers (1–3 installments)

Scale operations aggressively during Q4 (Nov peak)

🛠 Tech Stack

SQL (BigQuery)

Window Functions, CTEs

Date & Time Analysis

Aggregations & Joins
