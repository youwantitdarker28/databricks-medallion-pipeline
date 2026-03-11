# Databricks Medallion Architecture Pipeline

## Project Summary
A portfolio data engineering project built across two days in Databricks Free Edition. It downloads real CSV datasets from GitHub (datablist) and builds a full Medallion Architecture pipeline (Bronze → Silver → Gold) with incremental loading and audit logging using PySpark and Delta Lake.

## Workspace & Catalog Structure

**Workspace Structure:**
```text
Workspace/sathwik/
└── databricks_practice/
    ├── customers/     ← Day 1 work
    │   ├── 01_ingest_customers
    │   ├── 02_silver_customers
    │   └── 03_gold_customers
    └── people/        ← Day 2 work
        ├── 00_create_audit_table
        ├── 01_ingest_people
        ├── 02_silver_people
        ├── 02_silver_people_incremental
        └── 03_gold_people
