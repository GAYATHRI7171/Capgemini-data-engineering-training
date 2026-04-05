## Objective
The objective of this phase is to build an end-to-end data processing workflow using **PySpark** by implementing the **ETL (Extract, Transform, Load)** process and producing useful analytical insights from structured datasets.

---

## Project Overview
This project involves analyzing customer and sales data stored in different file formats including **CSV, JSON, and Parquet**.

### Key Activities:
- Ingested data from multiple data sources
- Performed data cleansing and validation
- Applied transformations and aggregations
- Generated analytical reports such as sales trends and revenue analysis
- Identified high-value and returning customers

---

## Implementation Approach
- Loaded datasets into PySpark DataFrames
- Inspected schema and sample data using `printSchema()` and `show()`
- Cleaned datasets by removing null and inconsistent records
- Processed data across CSV, JSON, and Parquet formats
- Applied joins and aggregation logic to derive insights
- Implemented window functions for ranking and advanced analysis

---

## PySpark Operations Used
- `groupBy()` and `agg()` → Aggregation operations
- `join()` → Dataset merging
- `filter()` and `dropna()` → Data cleaning
- `withColumn()` and `when()` → Column transformations
- Window functions → Ranking and analytical computations

---

## Generated Outputs
The following analytical results were produced:
- Daily sales performance report
- Revenue analysis by city
- Identification of repeat customers
- Top-performing customer in each city
- Consolidated final analytical dataset

All generated outputs are stored inside the **`OUTPUTS/`** directory.

---

## Challenges Faced
- Managing missing and inconsistent data entries
- Understanding and implementing window functions
- Handling datasets from multiple file formats
- Applying correct transformation logic during ETL processing

---

## Key Learnings
- Designed an end-to-end ETL pipeline using PySpark
- Enhanced skills in data validation and preprocessing
- Worked with heterogeneous data sources (CSV, JSON, Parquet)
- Learned advanced analytics using window functions

---

## Repository Structure
- `solution/` → PySpark ETL implementation scripts  
- `phase3_problem_statement/` → Project problem details  
- `OUTPUTS/` → Result screenshots and reports  
- `README.md` → Project documentation
