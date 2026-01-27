# 🚀 Azure Databricks End-to-End Data Engineering Project

## 📌 Overview
This repository contains a **production-style end-to-end data engineering project** built using **Azure Databricks**.  
The project demonstrates how modern data platforms are designed using **Medallion Architecture (Bronze, Silver, Gold)** with proper **governance, incremental ingestion, transformations, and analytics**.

The goal of this project is to replicate **real-world data engineering workflows** rather than a simple hobby or demo pipeline.

---
<img width="869" height="300" alt="1" src="https://github.com/user-attachments/assets/f12f2afc-3dd8-4a7e-b237-ee222b901119" />
<img width="942" height="368" alt="Capture" src="https://github.com/user-attachments/assets/71f0cf6e-7539-4cb3-aed4-409b162b847e" />
<img width="1536" height="1024" alt="ChatGPT Image Jan 21, 2026, 10_34_10 AM" src="https://github.com/user-attachments/assets/5b9797b6-8b76-472d-9e52-e43c4da16478" />

<img width="803" height="401" alt="3" src="https://github.com/user-attachments/assets/a6518f7e-1419-4a8f-beee-a949e457f0df" />
<img width="957" height="423" alt="2" src="https://github.com/user-attachments/assets/558089c3-ffad-478f-a165-e58da325d879" />

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
Followed in DBC FILE


---

## 📦 Import Project into Databricks (DBC)

This repository provides a **DBC (Databricks Archive) file** so you can easily import the entire project.

### Steps to Import
1. Open your **Databricks Workspace**
2. Go to **Workspace**
3. Click **Import**
4. Upload the `.dbc` file from the `dbc/` folder
5. Import into your desired workspace directory

Once imported, all notebooks will be available in the same structure as the project.

---

## ▶️ How to Run the Project

1. Configure Azure Data Lake Gen2
2. Create Databricks workspace
3. Enable Unity Catalog and assign metastore
4. Create external locations for:
   - Source
   - Bronze
   - Silver
   - Gold
5. Run notebooks in order:
   - Bronze ingestion
   - Silver transformations
   - Gold modeling
6. Execute workflows for end-to-end orchestration
7. Query data using Databricks SQL Warehouse

📄 Detailed steps are available in:  
👉 `docs/setup.md`

---

## 💰 Cost Control & Best Practices

- Auto-terminate clusters (5–10 minutes)
- Use smallest node sizes
- Stop SQL Warehouses when not in use
- Keep storage, stop compute
- Delete unused resources

📄 More details in:  
👉 `docs/cost_control.md`

---

## 🎯 Interview Readiness

This project is intentionally designed to cover **frequently asked interview topics**, including:

- Medallion Architecture
- Incremental ingestion & idempotency
- SCD Type 1 vs Type 2
- Delta Lake & DLT
- Unity Catalog governance model
- Cost optimization strategies
- Real-world Databricks architecture decisions

📄 See:  
👉 `docs/interview_qna.md`

---

## ⚠️ Notes on Azure Subscriptions

Some advanced Databricks features (Unity Catalog, DLT, Serverless SQL) may require a **Pay-As-You-Go Azure subscription**.  
Azure Student subscriptions may have feature limitations.  
This project reflects **real-world production architecture**, independent of subscription constraints.

---

## 📌 Who Should Use This Project?

- Aspiring Data Engineers
- Azure Databricks learners
- Candidates preparing for Data Engineer interviews
- Anyone wanting real-world Databricks hands-on experience

---

## 🧠 Final Note

This is **not a tutorial project**.  
It is a **production-inspired data engineering implementation** focused on architecture, governance, scalability, and cost awareness.

If you can explain this project confidently, you can explain **most real Databricks workloads** in interviews.

---

⭐ If this project helped you, feel free to star the repository and share feedback.


