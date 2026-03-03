🎮 GameZone Sales Data Cleaning (SQL Server)

📌 Overview
This project demonstrates data cleaning and transformation using SQL Server on a raw CSV sales dataset. The objective was to prepare the data for reliable analysis by correcting data types, handling missing values, removing duplicates, validating business rules, and ensuring accurate revenue calculations.

🛠 Tools
- SQL Server
- SSMS
- T-SQL

🔍 Key Data Cleaning Tasks
- Converted text-based dates to proper DATE format using TRY_CONVERT
- Handled missing values in categorical and numeric fields
- Removed duplicate records using ROW_NUMBER() and CTE
- Standardized text formatting for consistency
- Validated shipping logic (no shipment before purchase)
- Converted price column to DECIMAL(10,2) for accurate aggregation
- Verified total revenue using SQL aggregate functions

📊 Example Query
SELECT SUM(USD_PRICE) AS Total_Revenue
FROM gamezone_orders_data;

🎯 Outcome
The dataset is now clean, consistent, and analysis-ready, suitable for reporting, KPI calculation, and dashboard development.
