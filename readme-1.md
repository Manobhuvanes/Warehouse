# TechMart Data Warehousing Project

This project demonstrates how to set up a data warehousing solution using IBM Db2 Warehouse on IBM Cloud for the fictional company "TechMart." The project includes a simple database schema, data loading instructions, and an example SQL query for analysis.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Database Schema](#database-schema)
- [Data Loading](#data-loading)
- [Data Warehousing and Analysis](#data-warehousing-and-analysis)
- [Sample Database Output](#sample-database-output)

## Prerequisites

Before you begin, ensure you have the following prerequisites in place:

- An IBM Cloud account.
- An instance of IBM Db2 Warehouse provisioned on IBM Cloud.
- Db2 Warehouse client tools installed on your local machine if needed for data loading and analysis.

## Getting Started

1. Create an instance of IBM Db2 Warehouse on IBM Cloud.
2. Use the provided connection details to connect to your Db2 Warehouse instance.

## Database Schema

The database schema for this project includes three tables: PRODUCTS, CUSTOMERS, and SALES. Here is the schema:

- `PRODUCTS`: Stores information about products available in TechMart.
- `CUSTOMERS`: Contains data about TechMart's customers.
- `SALES`: Records sales transactions, including product, customer, and purchase details.

## Data Loading

You can load data into the tables using various methods, such as the Db2 LOAD utility, SQL INSERT statements, or ETL tools. You need to populate these tables with real data for meaningful analysis.

## Data Warehousing and Analysis

With your data loaded, you can perform data warehousing tasks such as creating data marts, data transformation, and running analytical queries. An example SQL query to find total sales for a specific product is provided in the README.

## Sample Database Output

In the README, you will find sample data for the `PRODUCTS`, `CUSTOMERS`, and `SALES` tables. Additionally, there is an example SQL query to calculate the total sales for each product.

### Sample Database Output

**PRODUCTS**:

| PRODUCT_ID | PRODUCT_NAME | PRICE |
|-----------|--------------|-------|
| 1         | Laptop       | 800   |
| 2         | Smartphone   | 400   |
| 3         | Monitor      | 200   |

**CUSTOMERS**:

| CUSTOMER_ID | CUSTOMER_NAME |
|------------|---------------|
| 101        | Alice         |
| 102        | Bob           |
| 103        | Carol         |

**SALES**:

| SALE_ID | CUSTOMER_ID | PRODUCT_ID | SALE_DATE  | QUANTITY | TOTAL_AMOUNT |
|--------|------------|------------|------------|----------|--------------|
| 1      | 101        | 1          | 2023-10-01 | 2        | 1600         |
| 2      | 102        | 2          | 2023-10-02 | 3        | 1200         |
| 3      | 103        | 3          | 2023-10-03 | 4        | 800          |

**Query Result**:

| PRODUCT_NAME | TOTAL_SALES |
|--------------|-------------|
| Laptop       | 1600        |
| Smartphone   | 1200        |
| Monitor      | 800         |

Modify this README file as needed to provide detailed information about your TechMart data warehousing project, including data loading, analysis, and any specific instructions or customization for your environment.
