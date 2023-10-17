# Real-Time Stock Market Data Analysis 

## Overview

This project demonstrates the real-time analysis of stock market data using Amazon Web Services (AWS) infrastructure, Apache Kafka, and Python. The project focuses on processing real-time data from the NIFTY 50 stock market using a producer-consumer architecture, storing the data in Amazon S3, and enabling data querying using S3 SQL or Amazon Athena.

## Technologies Used

- **AWS (Amazon Web Services)**: This project leverages AWS services for scalable, reliable, and cost-effective infrastructure.
- **Apache Kafka**: Kafka is used for ingesting and distributing real-time stock market data.
- **Python**: The code for both the producer and consumer is written in Python, a versatile and widely used programming language.
- **NIFTY 50 Dataset**: The project utilizes the NIFTY 50 dataset for real-time stock market data analysis.

## Project Components

### 1. Amazon EC2 Instances

- This project uses Amazon EC2 instances to run both the Kafka producer and consumer.
- EC2 instances provide a scalable and easily configurable environment for real-time data processing.

### 2. Apache Kafka

- Kafka is used for message queuing and streaming.
- The producer collects real-time stock market data and sends it to Kafka topics.
- The consumer subscribes to these topics, processes the data, and performs real-time data analysis.

### 3. Data Resampling

- Data resampling is implemented in the consumer code to obtain different values of stock prices.
- This analysis is part of the project's real-time data processing.

### 4. Amazon S3

- Real-time stock market data is stored in Amazon S3 buckets.
- S3 is a highly scalable and durable storage solution, ensuring data integrity and accessibility.

### 5. Querying Data

- The stored data can be queried using S3 SQL queries or through Amazon Athena.
- S3 SQL and Amazon Athena provide flexible querying options for deriving insights from the collected data.

## Prerequisites

Before running this project, you will need:

- An AWS account with necessary permissions for EC2, Kafka, S3, and Athena.
- Kafka installed and configured on your EC2 instances.
- Python environment with the required packages for Kafka integration and data analysis.
- The NIFTY 50 dataset or access to a data source providing real-time stock market data.

## How to Run

1. Set up your Amazon EC2 instances for Kafka producer and consumer.
2. Configure the producer to collect real-time stock market data from the NIFTY 50 dataset and send it to Kafka.
3. Configure the consumer to subscribe to Kafka topics, perform data analysis, and store the results in Amazon S3.
4. Schedule data analysis tasks or real-time processing as needed.
5. Use S3 SQL or Amazon Athena to query and analyze the stored data.
