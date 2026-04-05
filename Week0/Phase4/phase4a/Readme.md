# PySpark Customer Segmentation Project – Phase 4A

## 1. Objective
The purpose of this phase is to implement **customer segmentation and bucketing techniques** using PySpark to transform continuous numerical data into meaningful analytical categories.

---

## 2. Project Overview
This project analyzes customer and sales datasets to perform behavioral segmentation by:

- Computing total spending per customer
- Measuring order frequency
- Applying multiple segmentation strategies
- Evaluating how different segmentation approaches influence analytical outcomes

---

## 3. Implementation Strategy

### Data Preparation
- Imported customer and sales datasets from CSV files into PySpark DataFrames
- Inspected schema and sample records using `show()` and `printSchema()`
- Joined datasets using the `customer_id` key
- Created a combined `full_name` column using `concat_ws()`

### Aggregation Stage
- Calculated overall customer spending using `sum()`
- Computed total number of orders using `count()`

### Segmentation Methods Applied
- **Rule-Based Segmentation** using `when()` with predefined thresholds
- **Quantile Segmentation** using `approxQuantile()` for data-driven categorization
- **Bucketizer Segmentation** using Spark MLlib for range-based grouping
- **Window Function Ranking** using `percent_rank()` to assign relative customer positions

### Comparative Analysis
- Grouped customers according to assigned segments
- Compared customer distribution across segmentation techniques

---

## 4. PySpark Operations Used
- `groupBy()` and `agg()` → Aggregation calculations  
- `join()` → Dataset integration  
- `withColumn()` → Feature engineering  
- `when()` → Conditional segmentation rules  
- `approxQuantile()` → Dynamic threshold creation  
- `Bucketizer` → Numerical range bucketing  
- Window functions (`percent_rank()`) → Ranking analysis  

---

## 5. Output Insights
- Customer segmentation using multiple methodologies
- Distribution of customers across spending categories
- Quantile-based segmentation analysis
- Bucketized spending groups
- Rank-based customer performance evaluation

---

## 6. Data Engineering Practices
- Ensured schema correctness using `inferSchema`
- Prevented duplicate aggregations during joins
- Maintained consistent naming conventions
- Selected segmentation techniques appropriate for data distribution patterns

---

## 7. Challenges Encountered
- Understanding differences between segmentation strategies
- Implementing quantile calculations accurately
- Applying window functions for ranking analysis
- Comparing results produced by multiple approaches

---

## 8. Key Learnings
- Gained practical experience in customer segmentation techniques
- Understood fixed vs data-driven categorization methods
- Worked with Spark MLlib Bucketizer and window analytics
- Improved analytical thinking for customer behavior analysis

---

## 9. Repository Structure
- `solution/` → PySpark segmentation implementation  
- `phase4a_problem_statement/` → Project requirements  
- `OUTPUTS/` → Result outputs and screenshots  
- `README.md` → Project documentation
