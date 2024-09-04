# PySpark Jupyter Notebook Guide
This Jupyter Notebook demonstrates how to use PySpark in a Python environment without needing to install PySpark via `pip`. Instead, it leverages the existing Spark installation by setting the necessary environment variables and paths. This setup is essential for ensuring PySpark can be used seamlessly within the notebook.

## Table of Contents
1. Prerequisites for PySpark
2. Starting a SparkSession
3. Creating DataFrames
4. Viewing Data
5. Selecting and Accessing Data
6. Applying Functions
7. Grouping Data
8. Getting Data In/Out
9. Working with SQL

## Prerequisites for PySpark
The first code cell is crucial for configuring the environment to use PySpark. Instead of installing PySpark using `pip`, this notebook assumes that Spark is already installed on the system. It sets up the environment variables and modifies the `sys.path` to include the necessary Spark directories.

### Steps
1. **Import Libraries**: Import os and sys to handle environment variables and paths
2. **Set Enviornment Variables**:
    - `PYSPARK_PYTHON`: Points to the Python executable being used.
    - `spark_python`: Points to the Spark Python directory.
    - `py4j`: Points to the `py4j` library within the Spark installation.
3. **Add paths to** `sys.path`: Ensures that the Python interpreter knows where to find the Spark and `py4j` libraries.
4. **Verify Setup**: Print the updated `sys.path` to confirm that the paths are correctly set.

This configuration allows PySpark to be imported and used in subsequent cells without anny issues.

## Starting a SparkSession
Once the environment is set up, a SparkSession is created, which is the entry point for any Spark-related operations. This section illustrates how to start a new Spark session.

## Creating DataFrames
This section covers creating PySpark DataFrames from various data sources, including lists of Row objects and CSV files.

## Viewing Data
Learn how to inspect the contents of a DataFrame, including viewing the top rows, displaying data vertically, and printing the schema.

## Selecting and Accessing Data
This section demonstrates how to select specific columns or rows, create new columns, and filter data within a DataFrame.

## Applying Functions
Shows how to apply custom functions to DataFrame columns using Pandas UDFs.

## Grouping Data
Examples of grouping data and performing aggregate functions, such as avg(), are provided.

## Getting Data In/Out
Covers saving DataFrames to CSV and Parquet formats and reading them back.

## Working with SQL
Illustrates how to interact with DataFrames using SQL queries.

## Conclusion
This notebook serves as a practical guide for performing common data processing tasks using PySpark in a Jupyter environment without the need for additional PySpark installations. Make sure your Spark installation is properly configured before running the cells.

