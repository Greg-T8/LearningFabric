# Microsoft Fabric Learning Paths

<img src='images/20250704043916.png' width='750'/>

<!-- omit in toc -->
## Contents
- [Learning Path: Get Started with Microsoft Fabric](#learning-path-get-started-with-microsoft-fabric)
  - [What is Microsoft Fabric?](#what-is-microsoft-fabric)
    - [OneLake](#onelake)


## Learning Path: Get Started with Microsoft Fabric

Reference: https://learn.microsoft.com/en-us/training/paths/get-started-fabric/

### What is Microsoft Fabric?

It is an end-to-end analytics SaaS platform that provides a single, integrated environment for data professionals and the business to collaborate on data projects. Fabric provides a set of integrated services that enable you to ingest, store, process, and analyze data.

Fabric includes the following services:
- Data engineering
- Data integration
- Data warehousing
- Real-time intelligence
- Data science
- Business intelligence

| **Category**               | **Type**                                 | **Microsoft Fabric Commentary**                                                                                          |
| -------------------------- | ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| **Data engineering**       | Pipeline-oriented development            | Supports development through Lakehouse and Notebooks using Spark and Delta Lake for pipeline creation and orchestration. |
| **Data integration**       | ETL/ELT and data movement                | Enables data ingestion and transformation via Dataflows Gen2 and Data Factory experiences across diverse sources.        |
| **Data warehousing**       | Structured storage and querying          | Provides a managed SQL Warehouse with T-SQL support for traditional warehousing and high-performance querying.           |
| **Real-time intelligence** | Streaming and event-driven analytics     | Uses Real-Time Analytics for ingesting and analyzing live data streams, optimized for low-latency and time-series data.  |
| **Data science**           | Machine learning and predictive modeling | Facilitates exploration and modeling with Notebooks, ML tools, and Azure ML integration in a collaborative workspace.    |
| **Business intelligence**  | Visualization and decision support       | Offers robust reporting and dashboarding through Power BI for actionable insights and business decision-making.          |

#### OneLake

OneLake is Fabric's centralized data storage architecture that eliminates the need to move or copy data between systems.

OneLake is built on *Azure Data Lake Storage (ADLS)* and supports various data formats, including Delta, Parquet, CSV, and JSON.

Fabric uses *shortcuts*, which are references to files or storage locations external to OneLake, allowing you to access existing *cloud* data without copying it.

<img src='images/20250704045139.png' width='750'/>

