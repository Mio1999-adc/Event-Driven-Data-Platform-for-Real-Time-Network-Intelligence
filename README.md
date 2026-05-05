# 🚀 Event-Driven Data Platform for Real-Time Network Intelligence  
**(Serverless + Streaming Data Engineering Project)**

---

## 📌 Overview

This project implements a **production-style, end-to-end data platform** inspired by a **Serverless RAN Intelligent Controller (RIC)** architecture.

It demonstrates how to design and build a **modern data engineering system** that supports:

- Real-time (streaming) processing  
- Batch analytics  
- Serverless event-driven computation  
- Scalable data storage and querying  

The system simulates **network (RAN) events** and processes them through a **hybrid data pipeline** to generate insights and trigger intelligent actions.

---

## 🧭 Architecture

---

## 🧱 Key Components

### 1. Data Simulator (`data_simulator/`)
- Generates synthetic RAN events:
  - Mobility events
  - Traffic spikes
  - Network anomalies  
- Acts as the **data source** for the platform  

---

### 2. Ingestion Layer (`ingestion/`)
- Publishes events to streaming system  
- Handles serialization and topic management  

---

### 3. Streaming Layer (`streaming/`)
- Real-time processing of incoming events  
- Implements:
  - Congestion detection  
  - Anomaly detection  
  - Mobility tracking  

- Represents **Near-RT processing layer**

---

### 4. Batch Layer (`batch/`)
- Processes large-scale historical data  
- Computes:
  - Aggregations  
  - Feature engineering  
  - Reports  

- Represents **Non-RT analytics layer**

---

### 5. Orchestration (`orchestration/`)
- Manages workflows and scheduling  
- Coordinates:
  - Batch jobs  
  - Data updates  
  - Pipeline dependencies  

---

### 6. Serving Layer (`serving/`)
- Provides low-latency data access  
- Maintains system state:
  - Cell-level state  
  - User-level state  

- Supports APIs for querying processed results  

---

### 7. Data Warehouse (`warehouse/`)
- Stores structured analytical data  
- Includes:
  - Fact tables  
  - Dimension tables  
- Enables OLAP-style queries  

---

### 8. Serverless Layer (`serverless/`)
- Event-driven execution of functions  
- Handles:
  - Real-time alerts  
  - Policy decisions  
  - Dynamic actions  

- Core innovation: **serverless RIC behavior**

---

### 9. Monitoring (`monitoring/`)
- Tracks system performance  
- Includes:
  - Metrics collection  
  - Dashboards  
  - Observability tools  

---

### 10. Configurations (`configs/`)
- Centralized configuration for all services  

---

### 11. Documentation (`docs/`)
- Architecture diagrams  
- System design explanations  
- Data modeling decisions  

---

### 12. Tests (`tests/`)
- Unit and integration tests for components  

---

## 🧰 Tech Stack

### Core Technologies
- Apache Spark (batch + streaming processing)  
- Apache Kafka (event streaming)  
- Apache Airflow (workflow orchestration)  

### Storage & Warehousing
- Parquet / Data Lake  
- BigQuery or Snowflake  

### Serving & State
- Cassandra (distributed storage)  
- Redis (low-latency access)  

### Serverless
- AWS Lambda or Cloud Functions  

### Monitoring
- Prometheus  
- Grafana  

---

## ⚙️ Local Development

### Prerequisites
- Docker & Docker Compose  
- Python 3.9+  

### Start services
```bash
docker-compose up -d

