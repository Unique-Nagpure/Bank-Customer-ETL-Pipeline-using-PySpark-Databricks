# Bank-Customer-ETL-Pipeline-using-PySpark-Databricks
This project demonstrates an end-to-end ETL (Extract, Transform, Load) pipeline built using PySpark on Databricks to process raw banking customer data.

# Project Overview
The pipeline ingests raw customer data from Databricks Unity Catalog, performs comprehensive data validation and cleaning, applies business transformations, generates data quality metrics, and loads the curated dataset back into Unity Catalog for downstream analytics and reporting.

This project is designed to showcase practical Data Engineering skills, including large-scale data processing, data quality management, schema validation, transformation logic, and production-style ETL development using PySpark.

# Business Problem

Banks collect customer information from multiple branches and channels. Since the data originates from different sources, it often contains inconsistencies that can impact reporting, analytics, and regulatory compliance.

# The objective of this project is to build a robust ETL pipeline that:

Validates incoming customer records
Detects and removes duplicate records
Handles missing and invalid values
Standardizes customer information
Applies business transformations
Produces a clean and analytics-ready customer dataset
Technology Stack
PySpark
Apache Spark
Databricks
Unity Catalog
Spark SQL
Delta/Parquet Storage
Dataset

# The project uses a simulated banking customer dataset containing 103,000 records with intentional data quality issues to mimic production scenarios.

Dataset Columns
customer_id
first_name
last_name
gender
dob
email
phone
state
city
branch
income
account_type
created_date

# ETL Pipeline
Raw Customer Data (Unity Catalog)
            │
            ▼
      Data Ingestion
            │
            ▼
     Data Validation
            │
            ▼
      Data Profiling
            │
            ▼
      Data Cleaning
            │
            ▼
 Business Transformations
            │
            ▼
   Data Quality Reporting
            │
            ▼
 Curated Customer Dataset

# Data Validation
The pipeline performs several validation checks, including:

Schema validation
Record count verification
Duplicate customer detection
Null value analysis
Distinct value analysis
Descriptive statistics
Data Cleaning

# The following data quality improvements are applied:

Removed duplicate customer records
Standardized gender values
Normalized state names
Trimmed unwanted spaces
Validated email addresses using regular expressions
Standardized phone numbers
Handled missing income values
Converted multiple date formats into a consistent format
Business Transformations

# Additional business attributes are created, including:
Customer Full Name
Customer Age
Income Group
Customer Segment
Senior Citizen Flag
Account Age
Data Quality Metrics

# Summary 
The final output is a clean, standardized, and business-ready customer dataset stored in Databricks Unity Catalog, making it suitable for downstream reporting, analytics, and machine learning applications.
