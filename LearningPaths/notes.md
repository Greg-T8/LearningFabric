# Microsoft Fabric Learning Paths

<img src='images/20250704043916.png' width='750'/>

<!-- omit in toc -->
## Contents
- [Learning Path: Get Started with Microsoft Fabric](#learning-path-get-started-with-microsoft-fabric)
  - [What is Microsoft Fabric?](#what-is-microsoft-fabric)
    - [OneLake](#onelake)
    - [Workspaces](#workspaces)
    - [Administration and Governance](#administration-and-governance)
  - [Data Teams and Microsoft Fabric](#data-teams-and-microsoft-fabric)
    - [Traditional Roles and Challenges](#traditional-roles-and-challenges)
    - [Evolution of Collaborative Workflows](#evolution-of-collaborative-workflows)
  - [Enable and Use Microsoft Fabric](#enable-and-use-microsoft-fabric)


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

- OneLake is Fabric's centralized data storage architecture that eliminates the need to move or copy data between systems.
- OneLake is built on *Azure Data Lake Storage (ADLS)* and supports various data formats, including Delta, Parquet, CSV, and JSON.
- Fabric uses *shortcuts*, which are references to files or storage locations external to OneLake, allowing you to access existing *cloud* data without copying it.

<img src='images/20250704045139.png' width='750'/>

#### Workspaces

- Workspaces serve as logical containers that help you organize and manage your data, reports, and other assets. They provide a clear separation of resources and maintain security.
- Each workspace has its own set of permsisions.
- Workspaces allow you to manage compute resources and integrate with Git.

#### Administration and Governance

See [Microsoft Fabric Administration](https://learn.microsoft.com/en-us/fabric/admin/) documentation.

### Data Teams and Microsoft Fabric

#### Traditional Roles and Challenges
* Traditional analytics workflows are fragmented across roles, leading to coordination challenges and delays.
* Data engineers prepare data for analysts, but this handoff can cause misinterpretations and inefficiencies.
* Data analysts often need to perform extra data transformations, which are time-consuming and lack context.
* Data scientists struggle to integrate their techniques into complex systems, limiting their ability to deliver insights effectively.

#### Evolution of Collaborative Workflows

Microsoft Fabric simplifies the analytics development process by unifying tools into a SaaS platform. Fabric allows different roles to collaborate effectively without duplicating efforts.

**Data engineers** can ingest, transform, and load data directly into OneLake using Pipelines, which automate workflows and support scheduling. They can store data in lakehouses, using the Delta-Parquet format for efficient storage and versioning. Notebooks provide advanced scripting capabilities for complex transformations.

**Data analysts** can transform data upstream using dataflows and connect directly to OneLake with Direct Lake mode, reducing the need for downstream transformations. They can create interactive reports more efficiently using Power BI.

**Data scientists** can use integrated notebooks with support for Python and Spark to build and test machine learning models. They can store and access data in lakehouses and integrate with Azure Machine Learning to operationalize and deploy models.

**Analytics engineers** bridge the gap between data engineering and analysis by curating data assets in lakehouses, ensuring data quality, and enabling self-service analytics. They can create semantic models in Power BI to organize and present data effectively.

**Low-to-no-code users** and **citizen developers** can discover curated datasets through the OneLake Hub and use Power BI templates to quickly create reports and dashboards. They can also use dataflows to perform simple ETL tasks without relying on data engineers.

### Enable and Use Microsoft Fabric

To access the Fabric tenant settings, sign in to https://fabric.microsoft.com and select the **Settings** icon; then **Admin Portal**:

<img src='images/1751623590729.png' width='300'/>
