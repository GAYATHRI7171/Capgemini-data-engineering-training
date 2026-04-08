

🚀 Phase 6 – Spark Playground Exit Sprint (Advanced Practice Lab)
---
📌 Objective

Build fluency and confidence in PySpark by solving advanced data engineering problems involving:

Joins
Window functions
Date transformations
End-to-end pipeline execution

📊 Problem Summary

Worked with dirty datasets (customers, orders) containing:

Null values
Invalid records (negative amounts, incorrect foreign keys)
Duplicate data

🎯 Goals:

Clean and validate data
Perform joins between datasets
Apply aggregations and window functions
Build a complete data pipeline

⚙️ Approach

🔹 Data Ingestion
Loaded datasets into PySpark DataFrames

🔹 Data Cleaning
Removed null values from critical columns
Filtered invalid records (negative amounts)
Trimmed string columns
Removed duplicate records

🔹 Data Validation
Used left_anti join to detect invalid foreign keys
Ensured referential integrity

🔹 Data Transformation

Applied joins:

Inner join → valid records
Left join → validation
Performed aggregations:
Total customer spend
Order count

🔹 Window Functions

Ranked customers based on total spend
Calculated running totals
Applied lag operations

🔹 Date-Based Analysis

Converted to date using to_date()
Extracted month using month()
Aggregated monthly sales

🔹 Output

Generated and saved final processed dataset

🛠️ Key Transformations

join() → Combine datasets
left_anti join → Detect invalid keys
groupBy() → Aggregations
agg() → Sum, count calculations
filter() → Remove invalid data
dropna() → Handle nulls
dropDuplicates() → Remove duplicates
Window functions → Ranking & analytics
to_date(), month() → Date operations

📈 Results

Cleaned datasets (customers, orders)
Identified invalid foreign keys
Customer-level metrics (total spend, order count)
Ranked customers by spending
Monthly sales insights

🧩 Data Engineering Considerations

Performed cleaning before transformations
Ensured referential integrity using joins
Avoided duplicates after joins
Handled null and invalid values carefully
Validated outputs using counts and samples

⚠️ Challenges

Identifying invalid foreign keys
Handling messy real-world data
Understanding window functions
Managing complex transformation pipelines

🎯 Key Learnings

Advanced joins (inner, left, left_anti)
Importance of data validation
Practical use of window functions
Handling dirty datasets
Building end-to-end PySpark pipelines

🔮 Future Improvements

Performance optimization (caching, partitioning)
Automated data validation checks
Integration with Delta Lake / production pipelines
