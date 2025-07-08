## Project Overview

This project is based on a dataset originally designed for the 10alytics June Hackathon. Although I discovered the competition after the deadline, I choose to work on the data independently to enhance my data analytics and business intelligence skills.

The primary goal was to uncover key business insights from operational data and present them in a clean, dynamic, and decision-oriented Power BI report.

### [link to the project folder](https://drive.google.com/drive/folders/1119TcKVu4whV6Na7hwfQIffR9ACR5xSa) This folder contains screenshots of dashboard, pbix file, dataset, py file, ssms file.
---

## Data Collection, Cleaning & Transformation

- Loaded over 10 raw CSV files into a structured SQL database using Python for efficient handling and querying.
- Cleaned the dataset in SQL by:
  - Replacing special characters and normalizing inconsistent formats
  - Converting string-based datetime fields to proper `datetime` types and splitting them into separate date/time fields
  - Identifying and handling null or empty values (either replacing them with `"Unknown"` or removing unusable entries)
- Created SQL joins to discover frequently co-purchased products and streamline analysis.
- Built SQL views to isolate only the relevant and clean data required for Power BI modeling.

In Power BI:
- Generated a dynamic date table in Power Query to support time intelligence.
- Created calculated columns for bundling products, categorizing delivery delays, and labeling key customer and seller records.
- Defined DAX measures to calculate total revenue, total orders, average reviews, delivery performance, and more.
- Added a field parameter to allow dynamic switching between KPIs across multiple visualizations.

---

## Key Insights

- **Revenue Trends**: Identified monthly revenue patterns and seasonality across the business timeline.
- **Customer Behavior**: Highlighted top-performing customers by spend, while also identifying churn patterns across key cities.
- **Operational Efficiency**: Revealed delivery performance issues by location, helping isolate areas with consistent delays.
- **Product Strategy**: Uncovered high-performing product bundles and the impact of shipping cost on customer reviews and order volume.
- **Seller Performance**: Measured seller contributions by revenue and customer satisfaction (average review score).
- **Lead Analysis**: Provided insight into the most effective sources of qualified leads and their conversion value.

---

## Tools

- **Python** – Data ingestion and SQL database population  
- **SQL** – Data cleaning, normalization, and view creation  
- **Power BI** – Data modeling, DAX calculations, and dashboard development

---

## Outcome

This project demonstrates end-to-end capability in preparing, modeling, analyzing, and visualizing complex data for business decision-making. It reflects practical skills in using SQL and Power BI together to transform raw operational data into actionable insights.
