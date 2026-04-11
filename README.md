# E-Commerce-Sales-Data-Analysis
Analyzed 56K+ sales records, 25,164 orders, $24.91M revenue and 
$10.46M profit across 3 continents using AdventureWorks dataset. 
Faced performance issues handling large complex data — resolved by 
implementing Snowflake Schema which significantly improved model 
efficiency and query speed. Built DAX measures for Net Sales ($24M), 
Profit Margin (42%), Return Rate (2.17%) and YoY/MoM growth trends. 
Identified North America as the top performing continent ($9.4M net 
sales) and Bikes as the highest profit category ($9.7M). Segmented 
18K+ customers into 10 RFM groups revealing 3.34K disengaged and 
1.71K champion customers to support targeted marketing decisions.

---

## Tools & Technologies
- **Power BI** — Dashboard & Visualizations
- **Power Query** — Data Cleaning & Transformation
- **DAX** — Measures & Calculated Columns
- **Snowflake Schema** — Data Modeling

---

## Dataset
Source: AdventureWorks Sample Dataset

| File | Description |
|------|-------------|
| AdventureWorks Sales Data 2020-2022.csv | Sales data  |
| AdventureWorks Territory Lookup.csv | Sales territory and region information |
| AdventureWorks Customer Lookup.csv | Customer demographic and profile data |
| AdventureWorks Product Categories Lookup.csv |product category classifications |
| AdventureWorks Product Lookup.csv | Full product details including price and SKU |
| AdventureWorks Product Subcategories Lookup.csv | Product subcategory breakdown |
| AdventureWorks Returns Data.csv | Returned orders |

---
## Dashboard Preview

### Executive Summary
<img width="1556" alt="Executive Summary" src="https://github.com/user-attachments/assets/b646ffc2-fbb2-47db-be97-6729a500cc00" />

---

### Territory Wise Analysis
<img width="1544" alt="Territory Wise Analysis" src="https://github.com/user-attachments/assets/e67c3271-85bb-48ca-a0a4-25c86d111971" />

---

### Product Analysis
<img width="1560" alt="Product Analysis" src="https://github.com/user-attachments/assets/39e07b02-8046-4f5b-9255-23f556039a27" />

---

### RFM Segmentation — Customer Analysis
<img width="1557" alt="RFM Segmentation Customer Analysis" src="https://github.com/user-attachments/assets/37c1b651-dd19-416f-9844-73ab85775e77" />

## Data Processing & Methodology

### 1. Data Cleaning
- Handled missing and null values across all datasets
- Standardized inconsistent formats in customer, product, and Sales data
- Removed duplicate and irrelevant records to ensure data accuracy
- Applied all transformations using **Power BI Power Query (Transform Data)**

### 2. Data Modeling
- Structured tables following a **Snowflake Schema** approach:
  - **Fact Tables** — transactional data (sales, returns)
  - **Dimension Tables (dim)** — lookup data (customers, products, territory, categories,subcategory,date)
- Connected Fact and Dimension tables using **relationships** to:
  - Keep the data model lightweight and optimized
  - Improve dashboard performance and query speed
- Created a **new calculated Date/Calendar table** using DAX for time intelligence

### 3. DAX Measures
Written custom **DAX (Data Analysis Expressions)** measures to power the dashboard, including:
- Total Sales, Total Revenue, Total Orders,Netoff Sales
- Return Rate, Total Returns
- Month-over-Month and Year-over-Year growth
- RFM scores (Recency, Frequency, Monetary)
### 4 Territory wise Analysis
-Sales KPI accross region and continent.
### 5. RFM Customer Segmentation
Performed **RFM (Recency, Frequency, Monetary) Analysis** to segment customers based on:
- **Recency** — How recently a customer made a purchase
- **Frequency** — How often they purchase
- **Monetary** — How much they spend in total

Performed **RFM (Recency, Frequency, Monetary) Analysis** using DAX measures and calculated columns to classify customers into 10 segments: **Champions, Loyal, Promising, Potential Loyalist, Need Attention, About to Sleep, At Risk, Cannot Lose, Lost,** and **New/Low Value Customers.**
