# 🚖 NYC Taxi Data Pipeline – Azure Data Factory & Databricks

## 📖 Project Overview
This project demonstrates the design and implementation of an **end-to-end data engineering pipeline** for processing the **NYC Taxi dataset** using **Azure Data Factory (ADF)**, **Azure Databricks**, and **Azure Data Lake Storage (ADLS)**.

The pipeline automates data ingestion, transformation, and storage in an analytics-ready format. Business insights such as **vendor performance**, **payment trends**, and **trip distribution** were derived using Databricks.

---

## ❓ Problem Statement
The NYC Taxi dataset contains millions of trip records with diverse attributes (vendor IDs, payment methods, fares, trip distances, etc.).  
Challenges include:
- Raw data inconsistencies → not analytics-ready  
- Manual preparation → time-consuming and not scalable  
- Need for automation → to ensure **reliability, consistency, and efficiency**  

---

## 🎯 Objectives
- Ingest raw trip data into **Azure Data Lake Storage (ADLS)**  
- Automate pipelines in **Azure Data Factory (ADF)** with parameterization  
- Apply filtering, aggregation, and schema enforcement using **Mapping Data Flows**  
- Store curated datasets in **Parquet format** for scalability & performance  
- Analyze processed data in **Databricks notebooks**  
- Automate execution using scheduled triggers  

---

## 🏗️ System Architecture
**Components:**
- **Source**: NYC Taxi CSV (API endpoint)  
- **ADF Pipeline**: Copy Activity → Mapping Data Flow → Databricks Notebook  
- **Storage**: ADLS Gen2 with `raw/` and `processed/` layers  
- **Compute**: Azure Databricks  

---

## ⚙️ Implementation Details
1. **Configured Linked Services** → ADLS, Databricks, Integration Runtime  
2. **Defined Datasets** → Raw CSV & Processed Parquet  
3. **Copy Activity with Parameters** → Ingest data from API to `raw/`  
4. **Mapping Data Flow** → Transformations (filter, aggregate)  
5. **Databricks Analysis** → Business insights on processed data  
6. **Automation** → Weekly scheduled triggers  

---

## 📊 Results & Insights
✅ Automated pipeline ingests & processes millions of trip records  
✅ Processed data is stored in **Parquet format** for BI & analytics  
✅ Key findings:
- Vendor 2 handled ~60% of rides  
- Credit card payments = ~70% of revenue  
- Short trips (<2 miles) dominate rides  
- Evening peak hours observed  

---

## 💰 Cost & Service Comparison
- **Copy Activity** → Low-cost, bulk ingestion  
- **Mapping Data Flow** → Costlier, best for transformations  
- **Recommendation** → Use Copy Activity for ingestion & Data Flows for transformation  

---

## ☁️ AWS Equivalent
If implemented in AWS:
- **Storage** → S3  
- **Ingestion** → Glue, Lambda, or Data Pipeline  
- **Transformation** → Glue ETL or EMR Spark  
- **Analysis** → Databricks on AWS or EMR  
- **Triggering** → EventBridge, Step Functions  

---

## 📂 Repository Contents
- `README.md` → Project documentation (this file)  
- `Parth_ADF_NYC_Taxi_Pipeline.docx` → 📥 **Download this file to view the complete detailed project report**  


 

 
