## Objective
The main objective of this phase is to apply **PySpark data transformation techniques** and understand how real-world data processing is performed using concepts such as **joins, aggregations, filtering, and sorting**.

---

## Problem Overview
In this project, customer information and sales transaction datasets were analyzed to derive business insights using PySpark.

### Activities Completed:
- Computed overall spending for each customer
- Identified top performing customers based on purchase value
- Detected customers who have not placed any orders
- Generated revenue statistics based on city
- Calculated average transaction value per customer
- Found customers who placed multiple orders
- Ranked customers according to total purchase amount

---

## Methodology
- Imported datasets into PySpark DataFrames
- Performed data preprocessing and removed invalid records
- Executed aggregation operations to summarize data
- Applied join operations to combine customer and sales datasets
- Used filtering and ordering techniques to generate insights

---

## PySpark Operations Used
- `groupBy()` → Data grouping operations
- `agg()` → Aggregate calculations (sum, average, count)
- `join()` → Dataset integration
- `filter()` → Conditional data selection
- `orderBy()` → Result sorting
- `round()` → Precision handling for numerical values

---

## Results Generated
The analysis produced the following outputs:
- Customer-wise total expenditure
- Top customers based on spending
- Customers without purchase history
- City-level revenue analysis
- Average order value per customer
- Customers with repeated transactions
- Ranked customer spending report

All generated outputs are stored inside the **`outputs/`** directory.

---

## Data Engineering Practices Followed
- Eliminated null and inconsistent records
- Maintained standardized column naming conventions
- Applied rounding techniques for numerical accuracy
- Validated intermediate transformation results

---

## Challenges Encountered
- Handling similar column names across datasets
- Implementing correct aggregation logic
- Managing decimal precision during calculations
- Understanding different types of joins in PySpark

---

## Key Learnings
- Developed practical experience in PySpark transformations
- Improved understanding of joins and aggregation workflows
- Learned importance of data preprocessing and validation
- Strengthened end-to-end data processing skills
