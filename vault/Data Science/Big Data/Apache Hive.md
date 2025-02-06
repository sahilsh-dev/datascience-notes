
Hive is a data warehouse tool that enables SQL-like querying of structured and semi-structured data in Hadoop. It bridges the gap between SQL-based applications and the Hadoop ecosystem and uses HiveQL.

## Architecture

- **Metastore:** Stores metadata about tables and schemas.
- **Driver:** Parses and executes queries.
- **Query Engine:** Converts HiveQL queries into MapReduce jobs.
- **HDFS:** Stores the data queried by Hive.

![[Pasted image 20250206035752.png]]

## Features

- SQL-like query language (HiveQL).
- Scalability for large datasets.
- Integration with HDFS and other storage systems.
- Extensibility with custom functions. 

**Primary Use Case:** Data warehousing, ad-hoc queries, and data summarization.
**Language:** HiveQL (Hive Query Language), a SQL-like language.
**Purpose:** Hive simplifies data analysis on large datasets by enabling users familiar with SQL to query data stored in Hadoop without needing deep knowledge of MapReduce.

## Key Components

 1. Metastore:
	Central repository for metadata about Hive tables, partitions, columns, and their locations in HDFS.
	Typically backed by a relational database like MySQL, PostgreSQL, or Derby.
 2. Driver:
	Coordinates query execution and interacts with the query compiler and execution engine.
 3. Compiler:
	Compiles HiveQL queries into execution plans consisting of MapReduce, Tez, or Spark jobs.
 4. Execution Engine:
	Executes the query using MapReduce, Tez, or Spark frameworks in Hadoop.
 5. Query Interface:
	Tools for executing queries, such as Hive CLI, Beeline, or via JDBC/ODBC.

## Advantages:

- Simple learning curve for SQL users.
- Scalable and handles massive datasets efficiently.
- Flexible with various storage formats like ORC, Parquet, Avro, and text files.
- Extensible with UDFs and supports integrations with other Hadoop ecosystem tools.

## Disadvantages:

- Slower query performance compared to traditional RDBMS due to batch processing.
- Limited support for complex transactions.
- High latency for real-time queries.
