![[Pasted image 20250205221327.png]]

# Data Ingestion

**Definition:** The Data Ingestion Layer is responsible for collecting data from various sources and transferring it to the storage layer. This layer handles data from diverse sources such as IoT devices, social media, logs, databases, and more. 
Data ingestion can be batch (collected at scheduled intervals) or real-time (processed as it arrives). This layer must be scalable and able to process data at high velocity.

## Batch vs. Real-Time Data Ingestion

Batch ingestion processes data in chunks at periodic intervals, making it suitable for use cases like reporting and analytics on historical data.

Real-time ingestion, on the other hand, handles continuous streams of data and enables real-time analytics, making it essential for applications like monitoring and fraud detection. Tools like Apache Kafka, Apache Flume, and AWS Kinesis are widely used for both types of ingestion.

## Tools for Data Ingestion

Popular data ingestion tools include:

[[Apache Kafka]]: A distributed event streaming platform that handles real-time data feeds.
[[Apache Flume]]: A service for collecting, aggregating, and moving large amounts of log data.
AWS Kinesis: A fully managed service for real-time data streaming and ingestion. These tools ensure that data is reliably and efficiently ingested into the system.

---
# Data Storage Layer

The Data Storage Layer is responsible for storing vast amounts of raw data from the ingestion layer. The storage system needs to be scalable and capable of handling both structured and unstructured data. A good storage system also supports high availability, durability, and fault tolerance. This layer typically uses distributed storage systems to manage large datasets across multiple nodes.

## Types of Data Storage

There are several types of data storage used in Big Data systems:

**Distributed File Systems:** Examples include HDFS (Hadoop Distributed File System) and Amazon S3. These are designed to store large datasets across multiple machines.
**NoSQL Databases:** These are used to store semi-structured or unstructured data. Examples include Cassandra, MongoDB, and HBase.
**Relational Databases:** While less common in Big Data, they are sometimes used for structured data. Examples include MySQL and PostgreSQL.
**Data Lakes:** A centralized repository that stores vast amounts of raw data (structured, semi-structured, and unstructured) in its native format such as files, images, and videos.

---
# Data Processing Layer

The Data Processing Layer is where raw data is transformed into valuable insights. It involves the application of algorithms, data cleaning, aggregation, and computations. 
This layer includes both **batch processing and stream processing**, which are necessary to handle the two types of data flows (historical and real-time data). Processing at scale requires high-performance computing frameworks.

## Batch vs Stream Processing

**Batch Processing i**nvolves processing large volumes of data in scheduled batches. It is ideal for non-time-sensitive data and historical analytics.
**Stream Processing** handles real-time data as it flows through the system. It is used for time-sensitive applications, such as fraud detection, monitoring, and recommendation systems. Tools like [[Apache Spark]], [[Apache Flink]], and [[Apache Storm]] are widely used for stream processing.

## Data Processing Frameworks

**Apache Hadoop MapReduce:** A batch processing framework designed for large-scale data processing. It is highly scalable and fault-tolerant.
**Apache Spark:** An in-memory processing engine that supports both batch and stream processing. It is known for its speed and ease of use compared to MapReduce.
**Apache Flink:** A framework designed for real-time stream processing with low latency and high throughput.
**Google Dataflow:** A fully managed service for stream and batch data processing.
