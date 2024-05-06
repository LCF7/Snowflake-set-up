# snowflake-set-up
This repository demonstrates how to set up a basic data warehouse in Snowflake, complete with roles, warehouses, and schemas. It also includes scripts to create tables and import data from an external S3 bucket. The goal is to provide a foundational setup for data analytics and data processing in a Snowflake environment.

# Snowflake Data Warehouse Setup

## Overview

This repository demonstrates how to set up a basic data warehouse in Snowflake, complete with roles, warehouses, and schemas. It also includes scripts to create tables and import data from an external S3 bucket. The goal is to provide a foundational setup for data analytics and data processing in a Snowflake environment.

### Project Components

1. **Roles and Warehouses Setup**:
   - Creates three roles: `QA_ROLE`, `PROD_ROLE`, and `DBT_ROLE`.
   - Sets up three warehouses: `QA_WH`, `PROD_WH`, and `DBT_WH` (all with size `X-SMALL`).

2. **Database and Schema Setup**:
   - Creates two databases: `raw` and `analytics`.
   - `raw` has a schema named `source_1`, and `analytics` has two schemas, `prod` and `qa`.

3. **Tables Creation**:
   - Creates tables in the `raw.source_1` schema: `CUSTOMER`, `LINEITEM`, `NATION`, `ORDERS`, `PART`, `PARTSUPP`, `REGION`, and `SUPPLIER`.
   - Populates the tables using sample data from CSV files located in an S3 bucket.

### Repository Structure

- **Notebook**:
  - Contains all SQL scripts necessary to set up roles, warehouses, databases, schemas, and tables.
  - Demonstrates how to load data into tables from external sources.

- **Data**:
  - Example datasets (or links to them) used to populate the tables.

- **Scripts**:
  - SQL scripts used for setting up the Snowflake data warehouse and populating data.

### Getting Started

To use this project effectively:

1. Clone the repository locally.
2. Access your Snowflake account and create a database where you'll execute these scripts.
3. Modify the notebook or SQL scripts to include:
   - Your Snowflake account-specific details.
   - The paths to your S3 bucket containing the data.
4. Follow the instructions in the notebook to execute each script block in the right sequence.

### Prerequisites

- A Snowflake account with appropriate permissions to create and manage roles, warehouses, and databases.
- Access to sample data stored in an S3 bucket.
- Python and the Snowflake Connector for Python, if executing via a Jupyter notebook.

### Datasets

- Datasets provided are from snowflake data samples: SNOWFLAKE_SAMPLE_DATA.TPCH_SF1 limited to 10000 rows



