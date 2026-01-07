# 🚴 NOVAGEAR Retail Case Study – Power BI

## 📌 Project Overview

NovaGear Retail is a **multi-country specialty retail brand** selling bikes and cycling gear through both **online and physical stores**. This end-to-end Power BI case study focuses on transforming fragmented, multi-currency retail data into a **clean analytical model** and delivering **insight-driven dashboards** for business decision-making.

The project covers the full analytics lifecycle: **data ingestion → transformation → modeling → DAX → dashboarding → business insights**.

---

## 🧩 Business Problems Addressed

### 🔴 Problem 1: Inconsistent Sales Roll-ups

Sales reporting was inconsistent across regions due to:

* Multiple currencies
* Messy source systems
* Master-data inconsistencies

**Business need:**

* A unified **monthly USD view of sales**
* Analysis by **region, product hierarchy, and customer segment**
* A **clean star schema** for scalable future reporting

---

### 🔴 Problem 2: Limited Analytical Capability

Even after initial cleanup, the Fact table:

* Contained text fields
* Lacked time intelligence
* Could not support advanced KPIs or behavioral analysis

**Business need:**

* Robust time-based calculations
* Reusable measures and KPIs
* A strong analytical foundation

---

### 🔴 Problem 3: Lack of Interactive Reporting

Stakeholders needed:

* Executive-level insights
* Product performance visibility
* Customer trend analysis

**Business need:**

* Interactive dashboards with drill-downs, filters, and storytelling

---

### 🔴 Problem 4: Customer Retention & Behaviour Visibility

The business wanted to understand:

* Who is buying?
* Are we retaining customers?
* How customer behavior changes over time

This required **advanced DAX**, cohort-style logic, and meaningful visuals.

---

## 🗂️ Dataset Details

**Tables used (6):**

* Orders
* OrderLines
* Customers
* Products
* Stores
* ExchangeRates

These tables were combined and transformed to build a **central Fact Sales table**.

---

## 🔄 Data Transformation (Power Query)

* Connected and loaded multiple source tables
* Cleaned messy columns and fixed data types
* Handled multi-currency conversion using Exchange Rates
* Created a **central Fact table** from Orders & OrderLines
* Standardized keys for modeling

---

## 🧱 Data Modeling

* Designed a **Star Schema**
* Fact Table: Fact Sales
* Dimension Tables: Customers, Products, Stores, Calendar
* Correct cardinalities and relationships
* Optimized model for performance and accuracy

---

## 📅 Advanced Modeling & DAX Foundation

* Created a **Calendar table** for time intelligence
* Built calculated columns and helper tables
* Extracted and related columns across tables
* Created a dedicated **Measures Table** to manage all DAX measures

Key analytical capabilities added:

* YTD Sales
* Year-over-Year % Change
* 3-Month Rolling Average
* Period-based Retention Logic

---

## 📊 Dashboards Created

### 1️⃣ Executive Overview Dashboard

**Purpose:** High-level business performance

* KPI Cards: Total Sales, Profit, Profit Margin
* Sales & Profit trends
* Regional performance overview

Screenshot 2026-01-07 230744.png

---

### 2️⃣ Product Performance Dashboard

**Purpose:** Understand what is selling and where

* Product & category-level analysis
* Key Influencers visual
* Top-performing segments and regions

📸 *(Screenshot included in repository)*

---

### 3️⃣ Customer Insights Dashboard

**Purpose:** Customer trends and engagement

* Customer growth trends
* Segment-level behavior
* Drill-down analysis

📸 *(Screenshot included in repository)*

---

### 4️⃣ Retention & Behaviour Dashboard (Advanced Analytics)

**Purpose:** Deep customer behavior analysis

**KPI Cards (DAX-driven):**

* Active Customers
* Retention Rate (%)
* Purchase Frequency
* Average Order Value (AOV)

**Visuals:**

* Line Chart: Active Customer Trend
* Stacked Column: New vs Retained Customers
* Bar Chart: Top 10 Customers by Sales
* Table: Customer Performance Summary

**Advanced Features Used:**

* Drill-down & Drill-through (Customer-level)
* Tooltips for context
* Bookmarks & navigation
* Period-based retention logic

📸 *(Screenshot included in repository)*

---

## 🔍 Key Insights & Learnings

* Identified retention gaps across time periods
* Highlighted high-value customers driving revenue
* Observed purchase frequency patterns among retained customers
* Built meaningful business stories from raw data

This project involved **real analytical challenges**, especially in:

* Designing correct retention logic
* Interpreting trends across partial-year data
* Translating numbers into business-relevant insights

---

## 🛠️ Tools & Technologies

* Power BI Desktop
* Power Query (M)
* DAX
* Data Modeling (Star Schema)
* GitHub (Project Documentation)

---

## 📁 Repository Structure

```
NOVAGEAR-Retail-Case-Study/
│
├── Dataset/
│   └── Source_Data_Files
│
├── PowerBI/
│   └── NOVAGEAR_Retail.pbix
│
├── Screenshots/
│   ├── Executive_Overview.png
│   ├── Product_Performance.png
│   ├── Customer_Insights.png
│   └── Retention_Behaviour.png
│
└── README.md
```

---

## 👤 Author

**Pinkan Parida**
Aspiring Data Analyst | Power BI | SQL | Excel | Python

---

⭐ If you find this project insightful, feel free to star the repository
