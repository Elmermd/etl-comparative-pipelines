# ETL Comparative Pipelines with Pandas, PySpark and SQL

This repository contains a personal Data Engineering project focused on building and comparing **ETL pipelines** using **Pandas, PySpark, and SQL** over the **same datasets**.

The main goal is to demonstrate how identical data transformation logic can be implemented across different data processing engines while maintaining consistency in business rules and outputs.  
All pipelines are designed and executed within **Databricks**.

---

## Project Overview

The project follows a comparative approach:

- Same raw datasets (CSV files)
- Same transformation rules
- Same final outputs
- Different processing engines:
  - Pandas
  - PySpark
  - SQL (Databricks SQL / Catalog tables)

This approach highlights the strengths, syntax differences, and design considerations of each tool from a **Data Engineering perspective**.

---

## Technologies Used

- Python
- Pandas
- PySpark
- SQL
- Databricks (Community Edition)
- GitHub

---

## ETL Design Philosophy

Each ETL pipeline follows the same logical stages:

1. **Extract**
   - Read raw CSV files (clients, sales, etc.)
2. **Transform**
   - Data cleaning
   - Null handling (imputation or removal depending on the column)
   - Type casting
   - Deduplication
   - Business logic transformations
3. **Load**
   - Write clean datasets as CSV or tables
   - Outputs are separated by processing engine

For SQL pipelines, CSV files are loaded into Databricks and registered as tables in the catalog before applying transformations.

---

## Repository Structure

