# Apache Iceberg and Apache Hudi Demo

This project demonstrates the use of Apache Iceberg and Apache Hudi with Apache Spark. It provides a Docker-based environment to experiment with these technologies using PySpark and Jupyter notebooks.

## Overview

This project includes:

- **Jupyter Notebooks**: For interactive data processing and analysis.
- **PySpark**: Configured with dependencies for Iceberg and Hudi.
- **Data Warehouse**: Persistent storage for Iceberg and Hudi tables.

## Components

### Apache Iceberg

Apache Iceberg is an open table format for huge analytic datasets. It is designed to improve on the performance and usability of older Hadoop table formats like Hive and HDFS.

- **Features**:
  - Schema evolution
  - Partition evolution
  - Time travel queries
  - Hidden partitioning

### Apache Hudi

Apache Hudi (Hadoop Upserts Deletes and Incrementals) is a data lake platform that provides atomic upserts and incremental data streams on Big Data.

- **Features**:
  - ACID transactions
  - Record-level updates and deletes
  - Efficient data compaction
  - Incremental data processing

## Usage

### Iceberg Tables

Iceberg tables are created and managed using Spark SQL. The tables support schema evolution, partitioning, and time travel queries.

### Hudi Tables

Hudi tables are created and managed using Spark DataFrame API. The tables support ACID transactions, record-level updates, and efficient data compaction.

## Setup

1. **Docker Compose**: The environment is set up using Docker Compose, which includes services for PySpark and Jupyter notebooks.
2. **Jupyter Notebook**: Access the Jupyter notebook interface to run the provided notebooks and experiment with Iceberg and Hudi.

## Notebooks

The `notebooks/iceberg_hudi.ipynb` notebook demonstrates:

- Setting up Spark sessions for Iceberg and Hudi
- Creating sample data
- Writing data to Iceberg and Hudi tables
- Querying data from the tables

## Data Storage

The `warehouse/` directory contains the data for Iceberg and Hudi tables:

- `warehouse/iceberg/`: Stores Iceberg table data.
- `warehouse/hudi/`: Stores Hudi table data.

## Configuration

- **Spark Configuration**: The `spark-defaults.conf` file contains the necessary configurations for Spark to work with Iceberg and Hudi.
- **Docker Configuration**: The `docker-compose.yaml` and `Dockerfile.pyspark` files define the Docker environment for running PySpark and Jupyter notebooks.

## Conclusion

This project provides a comprehensive environment to explore and experiment with Apache Iceberg and Apache Hudi using Apache Spark. It demonstrates the capabilities and features of both table formats and how they can be used for efficient data processing and management.
