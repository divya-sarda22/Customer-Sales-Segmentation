# Customer Segmentation & Revenue Analysis

## Overview
End-to-end customer intelligence project using **RFM analysis** and **K-Means clustering**
on the UCI Online Retail dataset (541,909 transactions across 38 countries).

## Business Problem
How do we identify which customers are most valuable, which segments need attention,
and how much revenue is being lost through product returns?

## Dataset
- **Source:** UCI Online Retail Dataset
- **Size:** 541,909 transactions | 4,372 customers | 38 countries
- **Period:** December 2010 – December 2011

## Key Findings
- Identified distinct customer segments using RFM + K-Means clustering
- **£608,689 total revenue lost** due to 8,872 return transactions
- Top returned product: REGENCY CAKESTAND 3 TIER (180 returns)
- UK accounted for 7,501 returns — highest of any country
- Missing CustomerID handled for 135,080 records during data cleaning

## Methodology
1. **Data Cleaning** — handled 135,080 missing CustomerIDs, removed negative quantities
2. **EDA** — distribution analysis, correlation, country-wise breakdown
3. **RFM Feature Engineering** — Recency, Frequency, Monetary value per customer
4. **K-Means Clustering** — StandardScaler + Elbow method for optimal k
5. **Returns Analysis** — identified revenue loss, top returned products, return by country

## Tech Stack
- Python, Pandas, NumPy
- Scikit-learn (KMeans, StandardScaler)
- Matplotlib, Seaborn

## Business Impact
- Enables targeted marketing per customer segment
- Identifies £608K+ revenue loss from returns
- Highlights problematic products for quality improvement
- Supports data-driven decisions for customer retention

## How to Run
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
jupyter notebook customer_segmentation_pa.ipynb
```