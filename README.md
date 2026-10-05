# 📊 Global Super Store — Sales Dashboard (Power BI)

An interactive Power BI dashboard analyzing sales, profitability, returns, and regional performance for a fictional worldwide retailer, **Global Super Store**. Built as a hands-on business intelligence project on the classic *Superstore* dataset.

## 🎯 Project Overview

As the Sales Manager of Global Super Store, the goal is to analyze historical sales data to support inventory planning and business decisions, and to understand product and customer behavior.

### Key Metrics

| Metric | Value |
|---|---|
| Total Sales | $62.3M |
| Total Profit | $1.5M |
| Profit Ratio | 2.42% |
| Total Orders | 25,729 |
| Total Customers | 17,415 |
| Return Rate | 4.19% |

## 🗂️ Data Model

A star schema connecting one fact table to supporting dimension tables.

| Table | Rows | Role |
|---|---|---|
| Orders | 51,291 | Fact |
| Returns | 1,079 | Dimension |
| People | 25 | Dimension |
| Date Table | 1,461 | Date dimension |

### Relationships
- Orders[Order Date] → Date Table[Date] (Many-to-One)
- Orders[Region] → People[Region] (Many-to-One)
- Returns[Order ID] → Orders[Order ID] (Many-to-Many)

## 📐 Key DAX Measures


## 📊 Dashboard Features

- KPI Cards — Total Sales, Total Profit, Profit Ratio
- Sales Trend — monthly sales over 2012–2015
- Category & Segment Breakdown
- Sub-Category Performance table
- Regional profit contribution (donut)
- Interactive Market/Year slicer

## 🛠️ Built With

- Power BI Desktop
- Power Query (M)
- DAX

## 📝 Dataset

The Sample Superstore dataset, covering global retail orders from 2012–2015.

## 👤 Author

Ananthan S S
