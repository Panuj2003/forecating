# 🏨 Hotel Inventory Forecasting & Recommendation System

This project focuses on **forecasting the demand of bar inventory items** in a hotel using historical inventory movement data. The goal is to recommend optimal weekly par levels to reduce stockouts, prevent overstocking, and minimize wastage — ultimately improving operational efficiency.

## 📌 Business Problem

Hotels often face challenges in predicting how much inventory (like liquor, mixers, garnishes) to stock each week. Over-ordering leads to spoilage and wastage; under-ordering results in missed sales and dissatisfied customers.  
This system helps predict **weekly demand** using historical data and recommends **ideal par levels**.

## 🧠 Assumptions

- Historical consumption patterns reflect future trends.
- The data is clean and complete.
- Weekly time periods are suitable for inventory planning.
- External factors (like seasonality/events) remain mostly stable.

---

## 🔍 Methodology

We used **Simple Moving Average (SMA)** and **Rolling Mean** models to forecast weekly demand. These were chosen for:

- High interpretability
- Easy implementation
- Minimal computational requirements

## 📊 Dataset

- **Source:** Internal bar inventory records
- **Fields:** Item names, consumption quantities, dates, etc.
- **Granularity:** Weekly consumption totals 

## 📈 Forecasting Approach

1. **Data Cleaning** – Removing nulls, correcting data types, aggregating weekly.
2. **Exploratory Analysis** – Trend visualization per item.
3. **Forecasting** – Applying SMA with different window sizes.
4. **Par Level Recommendation** – Suggesting weekly ordering quantity based on forecast + buffer


