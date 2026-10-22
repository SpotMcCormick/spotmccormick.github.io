---
layout: default
title: Resume
---

## About

Data Engineer with experience building and productionizing cloud-native data pipelines across startup and enterprise environments. Skilled in designing scalable ETL/ELT workflows, serverless lakehouse architectures, and analytics-ready data models using AWS, DBT, Apache Iceberg, and modern CI/CD practices. Experienced integrating diverse data sources including APIs, IoT telemetry, geospatial, and vendor systems to support operational analytics, regulatory reporting, and business decision-making.

## Skills

- **Data Engineering:** Python, SQL, DBT, Apache Airflow, Apache Spark, Apache Iceberg
- **Cloud Platforms:** AWS (S3, Lambda, Athena, Glue, EC2), Terraform, Databricks (Delta Lake), GCP (BigQuery, Spanner)
- **Data Modeling:** Dimensional Modeling, Medallion Architecture, Data Lakehouse Architecture
- **Databases:** PostgreSQL, Snowflake, BigQuery, Neo4j, Azure SQL Server
- **Orchestration & CI/CD:** Airflow, GitHub Actions
- **Business Intelligence:** Tableau, Power BI, Looker, Streamlit, Dash
- **Other:** REST APIs, GeoPandas

## Work Experience

### Data Engineer (Contract), Townn, Remote
*May 2025 – July 2026*

- Designed near-real-time data ingestion workflows and **DBT** transformation pipelines for operational analytics, with automated **CI/CD** deployments to **GCP via GitHub Actions** and **Git**
- Implemented automated **DBT** unit testing workflows using **Python** Faker-generated synthetic application data and **DBT** fixtures in **GitHub Actions CI/CD**, enabling test-driven validation and automated merge approvals
- Collaborated with stakeholders to **define key reporting needs** and built initial dashboards in **Looker**, providing the first data-driven insights into core business operations
- Operated within an **Agile development environment**, managing and executing data engineering work tickets in **Jira** across sprints in a fast-paced startup setting

### Data Analyst, Atmos Energy, Jackson, MS
*October 2023 – Present*

- Built and **productionized** an end-to-end **ETL** pipeline (**Python, SQLite, Snowflake**) to automate the Damage Per Thousand metric; ingested vendor CSV reports via email parsing, staged data locally, and joined against warehouse damage data to generate operational KPIs that improved visibility into pipeline incident rates and decision-making
- Engineered a multi-source ETL pipeline (REST APIs + IoT sensor data) to support a corrosion risk model, enabling proactive identification of high-risk pipeline segments
- Developed and maintained data models in Azure SQL Server, supporting internal engineering workflows and project lifecycle tracking
- Designed and implemented a Neo4j graph database to model pipeline asset networks, improving traversal of infrastructure relationships and operational visibility
- Performed geospatial data processing (GeoPandas, ESRI API) to spatially relate pipeline assets, supporting graph modeling and field operations
- Developed operational metrics that contributed to a 56-day reduction in leak repair times, improving efficiency and regulatory performance
- Identified $80K in unaccounted capital, improving financial accuracy through data analysis

### Data Analytics Apprentice, Nashville Software School
*May 2023 – November 2023*

- Completed intensive full-time program; built ETL pipelines and performed data transformations using Python (Pandas, NumPy), queried relational databases with PostgreSQL, applied geospatial analysis with GeoPandas, ingested data via REST APIs and web scraping, and managed source control with Git/GitHub

### Owner/Educator, Spot's Drum Hub, Nashville, TN
*December 2016 – October 2023*

- Leveraged Google Analytics and MailChimp campaign data to track student engagement and optimize outreach, growing roster to 100 weekly clients

## Projects

### [AWS FMCSA Lakehouse](https://github.com/SpotMcCormick/aws-fmcsa-lakehouse)
*Personal Project, May 2026*

- Built and provisioned a fully serverless AWS lakehouse architecture using **Terraform**, deploying **Lambda** ingestion, **IAM policies**, **EventBridge** scheduling, **S3 storage**, and **Glue Catalog** resources entirely through infrastructure-as-code
- Engineered an automated monthly ingestion pipeline using **AWS Lambda** and **Python** to pull FMCSA carrier census data from the Socrata REST API into Amazon S3 as raw JSON bronze-layer storage
- Modeled a **medallion architecture** using **Athena, DBT**, and **Apache Iceberg** to transform raw API data into partitioned Parquet analytics tables optimized for downstream BI and reporting workloads
- Developed **Tableau** analytical marts aggregating active carrier counts, power units, and driver metrics by state, business organization type, and reporting year

### [World Flight Tracker](https://github.com/SpotMcCormick/world_flight_tracker)
*Personal Project, May 2026*

- Engineered an end-to-end medallion architecture pipeline ingesting near-real-time global flight telemetry from the OpenSky Network REST API into PostgreSQL as a raw JSON bronze layer, processing ~6.5M flight telemetry records daily
- Flattened and normalized JSON into structured data marts (silver layer) in PostgreSQL, then exported Parquet files every 5 minutes to Amazon S3 as the gold layer to support near-real-time analytical workloads
- Integrated Databricks Delta Lake to consume S3 Parquet data into ACID-compliant analytical views, implementing modern lakehouse architecture patterns using **Delta Lake**, columnar storage, and incremental refresh workflows

### [California Drought & Weather Correlation Tool](https://github.com/SpotMcCormick/ca-drought-weather-project)
*Personal Project, November 2025*

- Engineered a scalable AWS Data Lakehouse using Apache Iceberg to manage schema evolution and time-travel capabilities for multi-source environmental datasets
- Implemented a Medallion Architecture (Bronze, Silver, Gold) to orchestrate data refinement, utilizing Apache Iceberg for schema enforcement and ACID transactions across the data lakehouse
- Architected an automated ETL pipeline using **PySpark**, **Airflow**, and **DBT** to ingest and normalize **GeoJSON** (ca.gov) and REST API (Weather/Drought) data into a unified **S3**-backed storage layer
- Optimized query performance by implementing columnar storage and partitioning strategies, reducing data retrieval latency for downstream BI tools

## Education

**Bachelors in Science**, Liberty University, Lynchburg, VA (2024)
Majors: Business Administration & Data Analysis: Data Analytics

**Data Analytics Certificate**, Nashville Software School, Nashville, TN (2023)
Major: Data Analytics

<a class="button" href="/resume.pdf" download>Download Resume</a>
