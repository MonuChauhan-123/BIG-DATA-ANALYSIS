# BIG-DATA-ANALYSIS

# BIG-DATA-ANALYSIS TASK-1
COMPANY: CODTECH IT SOLUTIONS

NAME: CHAUHAN MONU MADANLAL

INTERN ID: CT12QVQ

DOMAIN: DATA ANALYSIS

DURATION: 8 WEEKS(January 30th, 2025 to March 30th, 2025.)

MENTOR: NEELA SANTOSH

### BIG DATA ANALYSIS USING PYSPARK
The notebook starts by installing PySpark using !pip install pyspark, ensuring that the required library is available for use. It then initializes a SparkContext (sc), which is the core engine that handles distributed data processing. The version of Spark is printed to verify the setup. After that, a SparkSession (spark) is created using SparkSession.builder.getOrCreate(), which is essential for working with structured data like DataFrames and SQL tables in Spark. The SparkSession acts as the entry point for all DataFrame-based operations.

The next section demonstrates how PySpark integrates with Pandas. It first creates a Pandas DataFrame (pd_temp) with 10 random values using NumPy. This DataFrame is then converted into a Spark DataFrame (spark_temp) using spark.createDataFrame(pd_temp), allowing large-scale processing. The notebook interacts with the Spark catalog, which manages metadata about tables. The command spark.catalog.listTables() is used to check the available tables before and after registering the DataFrame as a temporary table using createOrReplaceTempView("temp"). This allows SQL-style queries on the DataFrame, making it easier to analyze large datasets.

The final part of the notebook reads an external dataset (airports.csv) using spark.read.csv(file_path, header=True). This command loads the CSV file into a Spark DataFrame (airports), treating the first row as column headers. The dataset is then displayed using airports.show(), which prints the first few rows. This step showcases how PySpark can handle structured data from external files, making it suitable for big data analytics, ETL pipelines, and machine learning workflows.

Combining SQL and DataFrame APIs

PySpark allows seamless integration of SQL queries with DataFrame transformations.Both methods produce the same result but use different approaches.Both methods produce the same result but use different approaches.

