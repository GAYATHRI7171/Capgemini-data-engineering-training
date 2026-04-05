## Objective
This phase focuses on improving data quality by applying **data cleaning and preprocessing techniques using PySpark**. The goal is to prepare raw and inconsistent datasets for accurate analysis.

---

## Project Overview
In this project, a customer dataset containing missing values, duplicate entries, and incorrect records was analyzed and cleaned.

### Activities Completed:
- Detected null values and duplicate records
- Identified invalid or inconsistent data entries
- Applied cleaning techniques to improve dataset quality
- Verified cleaned data through validation checks
- Generated city-wise customer distribution

---

## Implementation Approach
- Imported the dataset into a PySpark DataFrame
- Examined data quality issues such as missing fields and invalid values
- Applied data cleaning operations:
  - Removed records with null `customer_id`
  - Replaced missing categorical values with `"Unknown"`
  - Eliminated duplicate records
  - Filtered rows with invalid age values (age <= 0)
- Verified dataset correctness using row count comparison
- Performed aggregation using `groupBy()` for analysis

---

## PySpark Operations Used
- `dropna()` → Remove rows containing null key fields
- `fillna()` → Replace missing values
- `dropDuplicates()` → Remove repeated records
- `filter()` → Exclude invalid data entries
- `groupBy()` → Group records by city
- `count()` → Calculate customer totals

---

## Results Achieved
- Successfully detected data inconsistencies
- Produced a cleaned and validated dataset
- Compared dataset size before and after preprocessing
- Generated customer count statistics for each city

---

## Data Engineering Practices
- Preserved primary key integrity (`customer_id`)
- Prevented analytical errors by removing duplicates
- Managed missing values without unnecessary data loss
- Ensured only valid records were used for analysis
- Validated transformations at each stage

---

## Challenges Encountered
- Identifying multiple categories of data quality issues
- Choosing appropriate strategies for missing values
- Maintaining data completeness during cleaning
- Understanding the impact of poor-quality data on analytics

---

## Key Learnings
- Real-world datasets require extensive preprocessing
- Data cleaning is a critical step in data engineering workflows
- Poor data quality directly impacts analytical outcomes
- Validation checks help ensure reliable results

---

## Repository Structure
- `pyspark_code/` → PySpark data cleaning scripts  
- `outputs/` → Generated output screenshots  
- `phase3a_problem_statement/` → Project requirements  
- `README.md` → Project documentation
