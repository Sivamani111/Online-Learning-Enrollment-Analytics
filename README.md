# Online Learning Enrollment Analytics Platform

## Project Overview
An end-to-end data engineering project built using **Databricks Lakeflow Spark Declarative Pipelines** and the **Medallion Architecture**.

The project processes online learning enrollment data through Bronze, Silver, and Gold layers to generate business insights and data quality reports.

## Technologies Used
- Databricks
- Apache Spark
- SQL
- Lakeflow Spark Declarative Pipelines
- Unity Catalog
- Medallion Architecture
- Databricks AI/BI Dashboards
- Genie

## Architecture

**Bronze → Silver → Gold → AI/BI Dashboard**

### Bronze Layer
- Ingested raw course enrollment CSV data.
- Created `bronze_course_enrollments`.

### Silver Layer
- Cleaned and standardized enrollment data.
- Handled duplicates and invalid records.
- Created:
  - `silver_enrollments_clean`
  - `silver_enrollments_rejected`

### Gold Layer
Created business-level summary tables:
- `gold_monthly_enrollments`
- `gold_category_summary`
- `gold_course_summary`
- `gold_channel_summary`
- `gold_data_quality`

### Dashboard
Created an interactive Databricks AI/BI Dashboard with three pages:
1. Overview
2. Courses & Channels
3. Data Quality

## Dataset
- File: `course_enrollments_raw.csv`
- Raw records: 1,283
- Expected clean records: 1,241

## Key Outcomes
- Built an end-to-end Medallion data pipeline.
- Implemented data cleaning and quality checks.
- Generated business-level analytical tables.
- Developed an interactive AI/BI dashboard.

## Author
Bala Siva Manikanta

## Dashboard Screenshots

### 1. Overview
<img src="<img width="1311" height="773" alt="Screenshot 2026-11-12 202117" src="https://github.com/user-attachments/assets/3bae6709-862c-4120-abfb-4a679b02f4d6" />
" width="100%">

### 2. Courses & Channels
<img src="screenshots/02_Courses_and_Channels.png" width="100%">

### 3. Data Quality
<img src="screenshots/03_Data_Quality.png" width="100%">

