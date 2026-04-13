🔹 Objective

In these phases, the goal is to perform analytical transformations on the cleaned dataset and store the final results for further usage.

This includes generating business insights such as top customers, repeat customers, and sales trends, and saving the outputs in an optimized format.

🔹 Problem Summary

After completing data cleaning, validation, and transformation, the task was to:

• Perform advanced analysis on sales data
• Identify top-performing customers
• Detect repeat customers
• Analyze monthly revenue trends
• Save the processed results for reporting and future use

🔹 Approach
Used cleaned and validated DataFrames from previous phases
Joined multiple tables (customers, cars, sales)
Created new calculated columns (revenue)
Applied aggregations and window functions
Generated analytical outputs
Saved results to storage in efficient formats
🔹 Key Transformations Used

• join() → to combine multiple tables
• withColumn() → to create derived columns (e.g., revenue)
• groupBy() → for aggregations
• agg() → to calculate metrics like sum and count
• row_number() (Window Function) → to rank customers
• filter() → to extract required results
• date_format() → for time-based analysis

🔹 Analysis Performed

✅ 1. Top 3 Customers per City
Used window function (ROW_NUMBER)
Ranked customers based on revenue within each city

✅ 2. Repeat Customers
Identified customers with more than one purchase
Used groupBy and count

✅ 3. Monthly Sales Trend
Extracted month from sale_date
Calculated total revenue per month
🔹 Output / Results

The following outputs were generated:

• Top customers per city
• Repeat customer list
• Monthly revenue trends

Formats used:
• Parquet (optimized for performance)
• CSV (for easy readability)

🔹 Data Engineering Considerations

• Used window functions instead of GROUP BY to retain detailed data
• Ensured aggregations are performed after cleaning
• Used efficient file formats like Parquet for storage
• Avoided data duplication during joins
• Verified outputs using sample checks

🔹 Challenges Faced

• Implementing window functions correctly
• Handling joins across multiple datasets
• Ensuring accurate revenue calculation
• Managing date formats for time-based analysis

🔹 Learnings

• How to perform analytical queries using PySpark
• Importance of window functions in real-world scenarios
• Difference between aggregation and window functions
• How to generate business insights from raw data
• Best practices for saving and storing big data outputs
