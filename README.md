# Customer Sales, Segmentation & Returns Analysis

## Project Overview

An end-to-end customer analytics project using Python, RFM analysis, K-Means clustering, and Power BI to understand customer purchasing behaviour, identify valuable customer segments, and analyse product return patterns.

The project uses the **UCI Online Retail Dataset**, containing 541,909 transaction records across 38 countries.

## Business Problem

How can a business identify its most valuable customers, understand customer purchasing patterns, identify customers who may need retention strategies, and investigate product returns?

## Dataset

- **Source:** UCI Online Retail Dataset
- **Original records:** 541,909 transactions
- **Unique customers before cleaning:** 4,372
- **Customers in final RFM analysis:** 4,339
- **Countries:** 38
- **Period:** December 2010 – December 2011

## Project Methodology

1. **Data Cleaning:** Handled missing CustomerIDs, removed duplicate records, converted invoice dates, and separated purchase records from return records.
2. **Exploratory Data Analysis:** Examined transaction data and prepared the purchase dataset for customer analysis.
3. **RFM Feature Engineering:** Calculated Recency, Frequency, and Monetary values for each customer.
4. **Feature Scaling:** Applied StandardScaler to prepare RFM features for clustering.
5. **K-Means Clustering:** Used the Elbow Method to select four clusters and applied K-Means to identify customer segments.
6. **Model Evaluation:** Evaluated clustering quality using the Silhouette Score.
7. **Returns Analysis:** Examined return records, return value, frequently returned products, and country-wise return patterns.
8. **Power BI Dashboard:** Created interactive reports covering sales performance, customer segmentation, and product returns.

## Customer Segments

The K-Means model identified four customer groups:

- **VIP Customers**
- **Loyal Customers**
- **At Risk Customers**
- **Low Value Customers**

## Key Findings

- Identified 4,339 customers for RFM analysis.
- Created four customer segments using K-Means clustering.
- Achieved a Silhouette Score of **0.616** for the four-cluster model.
- Identified 8,872 return records.
- Calculated a total return value of **-£608,689.47**.
- REGENCY CAKESTAND 3 TIER was the most frequently returned product, with 180 return records.
- The UK accounted for 7,501 return records, the highest among the countries analysed.

## Power BI Dashboard

The Power BI report contains three pages:

1. **Sales Overview:** Overall sales performance and key business metrics.
2. **Customer Analysis & Segmentation:** Customer distribution and RFM-based segments.
3. **Returns Analysis:** Return records, return value, frequently returned products, and country-wise return patterns.

### Dashboard Screenshots

Screenshots of all three report pages are available in the `Power BI/Screenshots/` folder.

## Tech Stack

- **Programming:** Python
- **Data Analysis:** Pandas, NumPy
- **Machine Learning:** Scikit-learn (K-Means, StandardScaler)
- **Model Evaluation:** Silhouette Score
- **Visualisation:** Matplotlib, Seaborn
- **Business Intelligence:** Microsoft Power BI
- **Development Environment:** Jupyter Notebook

## Business Applications

- Supports customer retention and targeted marketing strategies.
- Helps identify high-value and at-risk customer groups.
- Highlights products with frequent returns for further investigation.
- Provides interactive sales and customer performance reporting.
- Supports data-driven business decisions.

## Project Structure

```text
Customer-Sales-Segmentation/
│
├── Customer_segmentation_Analysis.ipynb
├── README.md
│
└── Power BI/
    ├── Revenue Segmentation Dashboard.pbix
    └── Screenshots/
        ├── Sales_Overview.png
        ├── Customer_Segmentation.png
        └── Returns_Analysis.png
```

## How to Run

1. Clone this repository.
2. Install the required Python libraries.
3. Place the UCI Online Retail dataset (`data.csv`) in the project root directory.
4. Open the notebook in Jupyter Notebook.
5. Run the notebook cells sequentially.

### Install Dependencies

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```