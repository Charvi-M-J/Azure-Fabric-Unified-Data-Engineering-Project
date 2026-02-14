# Azure-Fabric-Unified-Data-Engineering-Project
📌 Project Overview
This project implements a complete end-to-end Lakehouse data engineering pipeline using Microsoft Fabric, following the Medallion Architecture design pattern. Incremental data ingestion is handled using Autoloader, 
which efficiently loads new and modified files into the Bronze layer as raw Delta tables, ensuring scalable and optimized processing. In the Silver layer, data is cleaned, standardized, and enriched using PySpark
transformations, including lookup-based joins to integrate reference datasets and maintain data consistency. The Gold layer is designed using a Star Schema model, creating fact and dimension tables optimized for 
analytics and reporting. The entire pipeline is orchestrated using Microsoft Fabric Workflows, enabling automated, parameterized, and scalable execution for enterprise-level batch and near real-time data processing.
The solution implements:
• Incremental Data Ingestion using Autoloader
• Lookup-based Data Enrichment
• PySpark Transformations
• Medallion Architecture (Bronze → Silver → Gold)
• Star Schema Modeling
• Workflow Orchestration
• Delta Table Optimization

📸Screenshot
![image alt](https://github.com/Charvi-M-J/Azure-Fabric-Unified-Data-Engineering-Project/blob/a0f1deab42c20afed7ef1f414464deb479ea641f/screenshot/Screenshot%202026-02-13%20230253.png)

🏗 Architecture Overview
The pipeline follows Medallion Architecture:
  Source Files (CSV / Incremental Data)
        ↓
 Autoloader (Incremental Processing)
        ↓
 Bronze Layer (Raw Delta Tables)
        ↓
 Silver Layer (Cleaned + Lookup Enriched Data)
        ↓
 Gold Layer (Star Schema - Fact & Dimension Tables)
        ↓
 Fabric Warehouse / Power BI Reporting
 
🛠️ Technologies Used:
🔹 Microsoft Fabric – Unified platform for end-to-end data engineering and analytics
🔹 Lakehouse Architecture – Implements Medallion (Bronze, Silver, Gold) layered design
🔹 PySpark – Data transformation, cleaning, and enrichment logic
🔹 Apache Spark – Distributed big data processing engine
🔹 Delta Tables – ACID-compliant storage with optimized performance
🔹 Autoloader – Incremental file ingestion and scalable data loading
🔹 Fabric Workflows – Pipeline orchestration and automated execution

🎯 Key Learnings
• Designing scalable Lakehouse architectures using Medallion (Bronze, Silver, Gold) design
• Implementing incremental data ingestion using Autoloader for efficient file processing
• Configuring and optimizing Autoloader for scalable and near real-time data loads
• Performing distributed data transformations using Apache Spark and PySpark
• Applying lookup-based data enrichment to maintain referential integrity
• Creating business-ready Star Schema models for analytics and reporting
