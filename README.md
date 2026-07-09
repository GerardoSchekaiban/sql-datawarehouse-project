# sql-datawarehouse-project
## Project Overview

This project demonstrates how to build a modern SQL data warehouse from scratch using SQL Server. It covers the complete data warehousing process, from loading raw data to transforming it into a clean and structured model for reporting and analysis.

The project follows a layered architecture (Bronze, Silver, and Gold) to organize the data pipeline, apply data transformations, and create business-ready datasets using dimensional modeling.

By completing this project, I strengthened my understanding of data warehouse design, ETL processes, data modeling, and SQL development best practices.

## Architecture

This project follows the Medallion Architecture, which organizes the data warehouse into three layers:

* **Bronze:** Stores raw data extracted from the source systems as-is. This layer preserves the original data and serves as the foundation for the next stages.

* **Silver:** Cleans, standardizes, and transforms the raw data. Data quality checks and business rules are applied to create consistent and reliable datasets.

* **Gold:** Contains business-ready data modeled for reporting and analytics. This layer uses a star schema with fact and dimension tables to support analytical queries.
 <img width="756" height="569" alt="architecture" src="https://github.com/user-attachments/assets/ad65abfe-b62f-4d15-9d0d-91f04e70ad39" />


### Data Flow

The diagram below shows how data moves through the warehouse, from the source systems to the final analytical model. Each layer has a specific purpose, helping transform raw data into clean, business-ready datasets for reporting and analysis.
<img width="1416" height="669" alt="data-flow" src="https://github.com/user-attachments/assets/5bb891f1-3668-401b-a091-5624b64f0679" />


### Integration Model

Before building the dimensional model, data from the two source systems (CRM & ERP) is integrated into a unified view for each business entity. This step combines related data, with applied trasnformations, and creates consistent datasets that serve as the foundation for the final analytical model.
<img width="1413" height="690" alt="integration-model" src="https://github.com/user-attachments/assets/c5f1005f-7a55-4e85-9a41-0c79f599a9e3" />


### Data Model

The Gold layer is organized using a star schema to support reporting and analytical queries. It consists of a fact table (sales) and two dimension tables (customers and products), providing a simple and efficient structure for business analysis.

<img width="1470" height="527" alt="data-model" src="https://github.com/user-attachments/assets/5608d62d-a5c3-4fa4-adb6-c29e10e2c8e5" />




