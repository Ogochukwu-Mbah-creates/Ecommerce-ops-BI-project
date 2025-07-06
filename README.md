## Project Overview
This project was originally inspired by the 10alytics June Hackathon. Although I discovered the competition after the submission deadline, I decided to proceed with the dataset as a personal challenge to sharpen my skills in data cleaning, transformation, and business intelligence reporting using SQL, Python, and Power BI.

The objective was to simulate a real-world business case where multiple raw data sources must be consolidated, cleaned, and analyzed to extract valuable insights that drive decision-making.

---

## Data Collection

The dataset consisted of over 10 individual CSV files, covering various aspects of an e-commerce business—orders, deliveries, customers, products, and more. These files were programmatically ingested and loaded into a SQL database using Python for easier manipulation, cleaning, and integration.

---

## Data Cleaning & Transformation

After loading the data into SQL, I performed multiple cleaning and transformation steps to prepare it for analysis and visualization in Power BI.

### 🔧 Key Steps:

- **Standardization:** Replaced special characters and cleaned up inconsistent or incomprehensible symbols across the dataset to ensure data uniformity.

- **Datetime Handling:**  
  - Converted `VARCHAR` date/time fields to appropriate `DATETIME` types.  
  - Split combined datetime fields into separate `Date` and `Time` columns to support time-based analysis.

- **Missing Values Treatment:**  
  - Identified and flagged null or empty fields.  
  - Replaced missing values contextually (e.g., substituting "Unknown" for missing category names).  
  - Removed rows where values could not be reasonably inferred or replaced.

- **Relational Joins & Business Logic:**  
  - Used SQL joins to integrate related tables.  
  - Identified frequently co-purchased items to uncover product bundling patterns.

- **SQL Views for Optimized Analysis:**  
  - Created views that contain only the relevant, analysis-ready fields.  
  - This reduced model complexity and improved Power BI report performance by minimizing unnecessary data loading.

- **Power BI Enhancements:**  
  - Created a custom Date Table using `List.Dates` in Power Query to enable time intelligence features like YoY and MoM comparisons.  
  - Engineered calculated columns in Power BI, including:
    - A `Product Bundle` field from merged columns.
    - A `Delivery Status Category` column to classify delivery performance by city as "On Time", "Mild Delay", or "Severe Delay".
    - A region-based classification column to power filled map visuals for geographic delivery trends.

---

