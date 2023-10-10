# End-to-End Data Pipeline with Apache Kafka and AWS

This repository contains the code and configuration files for an end-to-end data pipeline built using Apache Kafka, ZooKeeper, and various AWS services. The pipeline is designed to ingest, process, store, and analyze stock market data in real-time. Below is an overview of the components and steps involved in this data pipeline.

## Components

### Apache Kafka and ZooKeeper

- Kafka is used for data ingestion and streaming.
- ZooKeeper is used to manage the Kafka cluster metadata.

### EC2 Instance

- The data pipeline is hosted on an EC2 instance, providing the infrastructure for data processing.

### Amazon S3 Bucket

- Data from Kafka is stored in an S3 bucket, providing scalable and durable storage for raw data.

### AWS Glue Crawler

- AWS Glue Crawler automatically discovers and catalogs metadata from the data stored in the S3 bucket.

### AWS Glue

- AWS Glue is used for Extract, Transform, Load (ETL) operations on the data.
- It transforms raw data into a structured format suitable for analysis.

### Database

- AWS Glue stores the transformed data in a database, which can be a relational database like Amazon RDS or a data warehouse like Amazon Redshift.

### Amazon Athena

- With the data cataloged by AWS Glue, Amazon Athena is used to run SQL queries on data stored in S3.
- Athena enables ad-hoc querying and real-time analysis of data.

## Getting Started

1. Install and configure Apache Kafka and ZooKeeper on the EC2 instance.
2. Set up an S3 bucket for data storage.
3. Use AWS Glue Crawler to catalog data.
4. Configure AWS Glue for ETL operations.
5. Store transformed data in a database.
6. Use Amazon Athena for real-time data analysis.


## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code according to the terms of this license.
