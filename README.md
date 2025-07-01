# ecommerce-pipeline-databricks


📌## Project Overview
This project demonstrates a complete end-to-end ETL pipeline and analytics solution using a large e-commerce dataset. The goal is to simulate a real-world data engineering workflow using Apache Spark on Databricks, where raw event data is ingested, cleaned, transformed, and analyzed to generate actionable insights.

We perform the following key steps:

Load a large raw CSV dataset into Databricks using Unity Catalog

Clean and transform the data using PySpark

Store the data as a Delta Table in Unity Catalog

Perform SQL-based data analysis and visualization

Build a dashboard to showcase business insights

Automate the ETL notebook using Databricks Jobs

## Technologies Used

| Technology                    | Purpose                                                 |
| ----------------------------- | ------------------------------------------------------- |
| **Databricks**                | Unified analytics platform for ETL, SQL, and dashboards |
| **Apache Spark (PySpark)**    | Data wrangling, transformation, and Delta Lake writing  |
| **Unity Catalog**             | Data governance and file storage management             |
| **Delta Lake**                | Reliable and scalable storage format                    |
| **SQL**                       | Business queries and metric extraction                  |
| **Databricks SQL Dashboards** | Interactive charts and KPI dashboards                   |
| **GitHub**                    | Version control and portfolio sharing                   |


## Dataset
Source: Kaggle E-Commerce Behavior Data

Size: ~2GB sampled from November 2019

Records: Millions of event-level interactions including view, cart, purchase

## ETL process
Data Upload

Uploaded raw CSV to Unity Catalog volume via Databricks interface

Data Cleaning & Transformation

Removed nulls from key columns like brand, category_code

Cast data types: price, product_id, user_id to appropriate types

Parsed and retained only meaningful columns

Data Storage

Stored cleaned data as a Delta Table named cleaned_events under workspace.ecomm schema


## Analytics & Dashboard

SQL Queries Included:
 Total number of purchases

Total items added to cart

 Revenue by product, brand, and date

 Daily purchase trends

 Top selling categories and products

 Most active users by interactions


 ##  Automation
 Created a Databricks Job that automatically runs the ETL notebook (Analysis notebook)

The job cleans, transforms, and updates the Delta Table on a scheduled or manual basis



