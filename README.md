#SQL Data Warehouse Project

#Project Overview

This project demonstrates the end to end development of a modern SQL Server data warehouse using a Medallion Architecture with Bronze, Silver, and Gold layers.

The project integrates data from CRM and ERP source files, applies data quality and transformation logic, and produces a business ready analytical model for reporting and analytics.

The main goal is to turn raw operational data into reliable, structured, and analytics ready data using SQL Server and SQL based ETL processes.

#Architecture

The project follows three main layers:

#Bronze Layer

The Bronze layer stores raw source data with minimal transformation.

Data is loaded from CSV source files into SQL Server using bulk loading techniques.

The main purpose of this layer is to preserve the source data and provide a reliable starting point for transformation.

#Silver Layer

The Silver layer cleans and standardizes the Bronze data.

Key activities include data cleansing, type conversion, duplicate handling, NULL handling, standardization, validation, and integration of CRM and ERP information.

The Silver layer prepares the data for reliable analytical modeling.

#Gold Layer

The Gold layer contains business ready data designed for analytics and reporting.

The data is organized using dimensional modeling with fact and dimension tables and a Star Schema approach.

The Gold layer provides a cleaner and easier structure for analytical queries and business reporting.

#ETL Flow

CRM and ERP CSV Files
        ↓
Extraction
        ↓
Bronze Layer
        ↓
Data Cleaning and Standardization
        ↓
Silver Layer
        ↓
Data Integration and Dimensional Modeling
        ↓
Gold Layer
        ↓
Analytics and Reporting

#Data Sources

The project uses data from two source systems:

1.CRM

Customer related information such as customer identifiers, names, demographic attributes, and creation information.

2.ERP

Business information related to customers, products, locations, and sales activity.

The two source systems are integrated in the warehouse to provide a unified analytical view.

#Data Warehouse Design

The Gold layer follows a dimensional modeling approach.

Dimension tables provide descriptive context such as customer, product, location, and date information.

Fact tables represent business events and quantitative measurements such as sales and transaction activity.

This design allows analytical questions such as:

Which products generate the most sales?

Which customers contribute the most revenue?

How do sales change over time?

Which product categories perform best?

#Key SQL and Data Engineering Skills Demonstrated

SQL Server
SQL
ETL
ELT concepts
Bulk data loading
Data cleansing
Data validation
Data standardization
Data integration
CTEs
JOINs
Aggregations
Window functions
CASE expressions
NULL handling
Date functions
String functions
Fact and dimension modeling
Star Schema
Medallion Architecture
Data warehouse design
Analytical SQL

#Tools and Technologies

SQL Server 2025 Express
SQL Server Management Studio
SQL
Git and GitHub
Draw.io
CSV datasets

#Data Quality

Data quality was treated as an important part of the transformation process.

The project handles common source data issues such as missing values, inconsistent formats, duplicate records, data type mismatches, invalid values, and inconsistent text representations.

The ETL process prepares the data before it reaches the analytical Gold layer.

#Learning Outcomes

This project provided practical experience with the complete warehouse development process, from source data ingestion to business ready analytical data.

It strengthened practical knowledge of SQL Server, SQL based ETL, data cleansing, data integration, dimensional modeling, fact and dimension tables, Star Schema, and Medallion Architecture.
