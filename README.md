# 🚀 Azure Databricks End-to-End Data Engineering Project

## 📌 Overview
This repository contains a **production-style end-to-end data engineering project** built using **Azure Databricks**.  
The project demonstrates how modern data platforms are designed using **Medallion Architecture (Bronze, Silver, Gold)** with proper **governance, incremental ingestion, transformations, and analytics**.

The goal of this project is to replicate **real-world data engineering workflows** rather than a simple hobby or demo pipeline.

---

## 🏗️ Architecture Overview

**High-level Flow:**

Source Data (Parquet)  
➡ Azure Data Lake Gen2  
➡ Azure Databricks (Bronze → Silver → Gold)  
➡ Delta Lake  
➡ Databricks SQL Warehouse  
➡ BI / Analytics (Power BI compatible)

### Key Architectural Concepts
- Medallion Architecture (Bronze, Silver, Gold)
- Separation of storage and compute
- Incremental ingestion & idempotent processing
- Data governance using Unity Catalog
- Analytics-ready star schema modeling

---

## 🧱 Technology Stack

| Layer | Technology |
|-----|-----------|
| Cloud Platform | Microsoft Azure |
| Processing Engine | Azure Databricks |
| Language | PySpark / SQL |
| Storage | Azure Data Lake Gen2 |
| File Format | Parquet, Delta |
| Governance | Unity Catalog |
| Orchestration | Databricks Workflows |
| Analytics | Databricks SQL Warehouse |

---

## ✨ Key Features Implemented

### 🔹 Data Ingestion (Bronze Layer)
- Incremental ingestion using **Spark Structured Streaming**
- Auto Loader for scalable file ingestion
- Idempotent data processing
- Raw data stored in Delta format

### 🔹 Data Transformation (Silver Layer)
- Advanced PySpark transformations
- Python OOP concepts integrated with PySpark
- Reusable logic via Unity Catalog functions
- Data cleansing and enrichment

### 🔹 Data Modeling (Gold Layer)
- Star Schema design
- Fact and Dimension tables
- Slowly Changing Dimensions:
  - Type 1 (PySpark implementation)
  - Type 2 (Delta Live Tables)
- Analytics-optimized Delta tables

### 🔹 Governance & Security
- Unity Catalog setup
- Metastore configuration
- External locations & credentials
- Fine-grained access control (catalog / schema / table level)

### 🔹 Analytics & Reporting
- Databricks SQL Warehouse
- SQL views for BI consumption
- Power BI–ready endpoints

---

## 📂 Repository Structure

