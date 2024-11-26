# Realtime Data Streaming | End-to-End Data Engineering Project

## Table of Contents
- [Introduction](#introduction)
- [System Architecture](#system-architecture)

---

## Introduction

I developed this project as a comprehensive guide to building an end-to-end data engineering pipeline. It covers every stage, from data ingestion to processing and finally to storage. I utilised a robust tech stack that includes:

- Apache Airflow
- Python
- Apache Kafka
- Apache Zookeeper
- Apache Spark
- Cassandra

To simplify deployment and scaling, I containerised the entire system using Docker.

---

## System Architecture

![image](https://github.com/user-attachments/assets/0cc0469f-c19d-40c4-8440-7c0fce763085)


I designed the system architecture to include the following components:

1. **Data Source**:
   - I used the `randomuser.me` API to generate random user data for the pipeline.

2. **Apache Airflow**:
   - I used Airflow to orchestrate the pipeline and store fetched data in a PostgreSQL database.

3. **Apache Kafka and Zookeeper**:
   - I leveraged Kafka and Zookeeper to stream data from PostgreSQL to the processing engine.

4. **Control Centre and Schema Registry**:
   - These components helped me monitor and manage schemas for Kafka streams.

5. **Apache Spark**:
   - I utilised Spark for data processing, setting up both master and worker nodes.

6. **Cassandra**:
   - I stored the processed data in Cassandra as the final destination.

---
