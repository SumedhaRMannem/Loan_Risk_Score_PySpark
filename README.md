# Loan Risk Score Calculation using Apache PySpark

## Project Description
This project focuses on data engineering and loan risk assessment for a consumer finance company that specializes in lending various types of loans to urban customers. The goal is to clean, process, and analyze large-scale loan data using Apache PySpark to help the institution make data-driven loan approval decisions.

## Problem Statement
Money lending institutions need to determine whether to approve or deny loan applications based on applicants' financial profiles. The challenge lies in ensuring that:

- **Low-risk applicants** get approved, preventing business losses due to unnecessary denials.
- **High-risk applicants** are rejected, minimizing financial losses due to loan defaults.

To achieve this, our data engineering team cleans and processes raw loan data to extract meaningful insights and calculate a **Loan Risk Score**.

## Key Features of the Project
✔ **Data Cleaning & Preprocessing**: Handling missing values, standardizing column names, and transforming data.  
✔ **Dataset Creation**: Breaking down the raw dataset into structured tables:
   - `customers_data`: Information about borrowers.
   - `loans_data`: Loan details.
   - `loan_repayments`: Loan repayment history.
   - `loan_defaulters`: Default history of borrowers.
✔ **Loan Risk Score Calculation**: Derived from:
   - Loan repayment history (**20%**)
   - Customer’s financial health (**35%**)
   - Loan defaulter records (**45%**)
✔ **Creating a Unified Data View**: Merging datasets for analytics.
✔ **Permanent Table & View Creation**: Enabling seamless SQL-based querying of the cleaned data.

## Dataset Details
- **Source**: Lending Club Dataset
- **Size**: 1.7 GB (CSV Format)
- **Records**: 2.26 million rows, 151 columns

## Processing Framework
- **Big Data Processing**: Apache Spark
- **Storage Format**: CSV & Parquet

## Tech Stack Used
- **Programming Language**: Python (PySpark)
- **Big Data Processing**: Apache Spark
- **Database**: Hive, Parquet
- **Storage**: HDFS
- **Visualization & Analytics**: Spark SQL