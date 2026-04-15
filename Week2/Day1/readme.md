
Insurance Data Analysis using PySpark & SQL
Project Overview

This project focuses on analyzing insurance data using PySpark and SQL to identify customer risk, validate data quality, and generate meaningful business insights.

The dataset includes:

Customers
Policies
Claims
Agents
Policy-Agent Mapping
Objectives
Perform data understanding and cleaning
Build relationships between datasets
Compute key business metrics
Identify high-risk customers
Apply advanced SQL concepts (Subqueries, CTE, and Window Functions)
Phase-wise Implementation
Phase 1 – Data Understanding

In this phase, the datasets were explored to understand their structure and relationships. Schema validation was performed to verify column types and ensure correctness.

Key checks included:

Identifying null values
Detecting negative or invalid values
Understanding how datasets are connected

The relationship flow was established as:

Customer → Policy → Claim → Agent

Phase 2 – Data Cleaning

This phase focused on improving data quality. Missing values were handled, and invalid entries such as negative premiums or claim amounts were removed.

Text columns were standardized to ensure consistency, and data types were corrected for proper analysis. Referential integrity checks were also performed to ensure that relationships between tables were valid.

Phase 3 – Transformations

In this phase, meaningful metrics were derived from the cleaned data.

Key calculations included:

Total premium per customer
Total claims per customer
Risk score (based on claim-to-premium ratio)

These transformations helped convert raw data into business-relevant insights.

Phase 4 – SQL Analysis (Including Subqueries)

This phase focused on performing analytical queries using SQL to extract insights from the data.

Business problems such as identifying top customers, repeat customers, and analyzing trends over time were solved.

🔹 Subqueries (Concept Added)

Subqueries were used to perform nested and dynamic calculations within a query.

A subquery is a query written inside another query and is useful when:

A calculation depends on another result
Filtering requires comparison with aggregated values
Data needs to be prepared before applying conditions

Different types of subqueries were applied, such as:

Scalar subqueries for single-value comparisons
Subqueries in filtering conditions for dynamic selection
Subqueries used to prepare aggregated data before joining

Subqueries made the queries more flexible and allowed solving complex problems in a structured way.

Phase 5 – Advanced SQL (CTE)

This phase introduced advanced SQL techniques to simplify complex logic and improve readability.

🔹 CTE (Common Table Expressions) – Concept Added

CTEs were used to break complex queries into smaller, manageable steps.

A CTE is a temporary result set that exists only during the execution of a query. It helps in organizing logic in a clear and structured way.

CTEs were mainly used for:

Performing intermediate calculations
Reusing results multiple times
Simplifying complex joins and aggregations

Multiple CTEs were also used together to perform layered transformations such as:

Aggregating customer-level metrics
Tracking latest activity (like last claim or order)
Combining multiple derived results into a final dataset

CTEs significantly improved readability compared to nested queries and made debugging easier.

Phase 6 – Window Functions

Window functions were used to perform calculations across a group of rows without collapsing them.

They helped in:

Ranking customers and agents
Comparing values across rows
Performing time-based analysis

Partitioning allowed grouping data logically (e.g., by city), and ordering enabled sequential calculations like trends and comparisons.

Phase 7 – Final Output

In the final phase, all processed and analyzed data was combined into a single dataset.

Additional derived columns such as risk indicators were added, and the output was stored in efficient formats for further use in reporting or dashboards.

Data Validation

Validation checks were performed to ensure data quality and accuracy:

Compared record counts before and after transformations
Verified that null values were handled correctly
Ensured no duplicate records existed
Maintained referential integrity across datasets
Key Insights
Identified high-risk customers based on claim behavior
Detected patterns and trends over time
Evaluated agent performance
Analyzed customer distribution across cities
Technologies Used
PySpark → Data processing and transformation
SQL → Analysis using Subqueries, CTE, and Window Functions
Parquet → Efficient data storage
Conclusion

This project demonstrates a complete data engineering and analytics workflow, including:

Data understanding
Cleaning and validation
Transformation
Advanced SQL analysis

The use of Subqueries, CTEs, and Window Functions enabled solving complex business problems efficiently and in a structured manner.
