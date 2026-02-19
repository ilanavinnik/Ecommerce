# 📊 E-Commerce Sales Dashboard (Power BI)

## Overview

Interactive Power BI dashboard analyzing e-commerce transaction data to generate actionable business insights.  
Designed to monitor revenue performance, customer behavior, product trends, and regional sales distribution.

---

## Dataset

**File:** `EcommerceData.csv`  
Transaction-level sales dataset including:

- Order ID & Order Date  
- Customer ID  
- Product / Category  
- Quantity  
- Sales / Revenue  
- Profit (if applicable)  
- Region / Segment  

---

## Key Features

- Interactive slicers (Date, Category, Region)
- KPI cards (Total Sales, Orders, Average Order Value)
- Revenue trend analysis (time-series)
- Category and product performance comparison
- Geographic sales visualization
- Drill-down functionality

---

## Data Modeling

- Structured data model with defined relationships  
- Fact and supporting dimension tables  
- Custom DAX measures for dynamic calculations  

Example:

```DAX
Total Sales = SUM(EcommerceData[Sales])
Average Order Value = DIVIDE([Total Sales], DISTINCTCOUNT(EcommerceData[Order ID]))
