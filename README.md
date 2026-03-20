# 🛒 E-commerce Data Warehouse

## 📌 Overview

This project builds an end-to-end **Data Warehouse system** for an E-commerce platform using modern data engineering practices.
It follows the **Medallion Architecture (Bronze → Silver → Gold)** to process, transform, and analyze data.

---

## 🏗️ Architecture

```
Raw Data → Bronze → Silver → Gold → BI Dashboard → Alerts
```

* **Bronze Layer**: Ingest raw data from source (CSV)
* **Silver Layer**: Clean, transform, and standardize data
* **Gold Layer**: Create business-level data models for analytics
* **BI Layer**: Dashboard visualization
* **Monitoring**: Detect anomalies in revenue

---

## ⚙️ Tech Stack

* Databricks
* Apache Spark (PySpark)
* SQL
* Delta Lake
* Git & GitHub

---

## 📂 Project Structure

```
ecommerce-data-warehouse/
│
├── Bronze_Define.ipynb        # Data ingestion
├── Silver_Define.ipynb        # Data cleaning & transformation
├── Gold_Modeling.ipynb        # Data modeling
├── Business_Reporting.ipynb   # Business queries
├── DashBoard_Thong_ke.json    # Dashboard
├── Alert_Doanh_thu.json       # Revenue anomaly alert
└── Set_up_catalog.ipynb       # Catalog & schema setup
```

---

## 🚀 Data Pipeline

### 1. Bronze Layer

* Load raw CSV data into Delta tables
* Add metadata: `ingestion_date`, `source_file`

### 2. Silver Layer

* Handle missing values
* Normalize schema
* Join datasets

### 3. Gold Layer

* Build fact & dimension tables
* Optimize for analytics queries

---

## 📊 Business Insights

* Revenue analysis by time
* Order trends
* Customer behavior
* Product performance

---

## 🚨 Alert System

* Detect abnormal revenue changes
* Trigger alert when:

  * Growth rate > 30%
  * Growth rate < -20%

---

## 📈 Dashboard

* Visualize key metrics:

  * Revenue
  * Orders
  * Growth rate
* Built for business users

---

## 🎯 Key Features

* End-to-end data pipeline
* Medallion architecture
* Scalable design
* Real-time monitoring (alert system)

---

## 📌 Future Improvements

* Add streaming data (Kafka)
* Implement Airflow for orchestration
* Optimize performance with partitioning
* Deploy on cloud (AWS/Azure)

---

## 👨‍💻 Author

* Nguyen Tien Dat
* Data Engineer (Aspiring)
