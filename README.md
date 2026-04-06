# Azure-Data-Engineering-Pipeline
Designed and implemented a complete Medallion Architecture (Bronze → Silver → Gold) using Azure Data Factory, Azure Data Lake, and Databricks — culminating in a fully functional Star Schema with Dimension and Fact tables ready for analytics.

### Data Overview
<img width="1786" height="612" alt="1 - Data Overview" src="https://github.com/user-attachments/assets/3e950b3b-e972-49be-afef-f77ea519effb" />

### Resource Group
<img width="1913" height="622" alt="2 -The Resource Group" src="https://github.com/user-attachments/assets/b945c6d5-cb0d-427e-94ec-0f84f414eba5" />


## What I Built
- Created end-to-end pipelines using Azure Data Factory + SQL Database
- Designed incremental data loading using watermark logic
- Stored and processed data in Azure Data Lake (Bronze, Silver, Gold layers)
- Loaded and transformed data using Databricks (PySpark)
- Built a clean, structured Silver layer with transformations and validation
- Designed Gold layer with Dimension & Fact tables (Star Schema)
- Implemented SCD Type 1 (Upsert) and Surrogate Keys for dimension management
- Automated workflows using Databricks Jobs & Pipelines


## Project Flow

1. Data is ingested from the source using Azure Data Factory
2. Initial load is stored in Azure SQL Database
3. Incremental pipeline loads only new data into the Data Lake (Bronze)
4. Data is cleaned and transformed into the Silver layer using Databricks
5. Business-level transformations create Gold layer tables
6. Dimension and Fact tables are built using the Star Schema design
7. Pipelines are orchestrated using ADF and Databricks Jobs

<img width="1024" height="1536" alt="workflow" src="https://github.com/user-attachments/assets/35f88216-d733-4d99-a517-f96795c8d5d2" />


## Full Cycle Pipeline run
<img width="1913" height="892" alt="10 1 - Full Cycle PipeLine run (in Databricks)" src="https://github.com/user-attachments/assets/bc60733c-9891-4511-813f-d3e41f420876" />


## ADF Pipeline
<img width="1917" height="691" alt="10 2 - ADF Pipeline" src="https://github.com/user-attachments/assets/5f4b34a9-ed1e-4e94-a4d9-e5c33e91420a" />



