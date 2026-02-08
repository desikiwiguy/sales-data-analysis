# Data Model Description

## Dataset Overview
The dataset consists of transactional retail sales records.  
Each row represents a single product purchased within an order.

This means the data granularity (level of detail) is:
**one row = one product in one order**

---

## Columns Used

- Order ID : Unique identifier for each order
- Order Date : Date when the order was placed
- Ship Date : Date when the order was shipped
- Region : Sales region (East, West, Central, South)
- Category : Main product category
- Sub-Category : Specific product type
- Sales : Revenue generated from the transaction
- Quantity : Number of units sold
- Profit : Profit earned from the transaction
- Customer Segment : Consumer / Corporate / Home Office

---

## Data Preparation Steps

The following preprocessing steps were performed before analysis:

1. Removed null or blank values
2. Converted date columns to proper date format
3. Standardized category names
4. Checked duplicate order IDs
5. Created date hierarchy (Year → Quarter → Month)

---

## Data Modeling

A single fact table was used for analysis.

Date hierarchy enabled:
- Monthly trend analysis
- Quarterly comparison
- Yearly performance tracking

Measures were created using DAX instead of calculated columns to improve performance.

---

## Analytical Purpose

The data model allows answering business questions such as:

- Which products generate the most revenue?
- Which categories generate loss?
- Which region performs best?
- Are sales seasonal?
- What is the profit margin?
