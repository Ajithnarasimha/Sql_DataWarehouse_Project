# 🏗️ Data Warehouse and Analytics Project

Welcome to the **Data Warehouse and Analytics Project** repository! 🚀

This project demonstrates a comprehensive data warehousing and analytics solution — from building a data warehouse to generating actionable insights. Built as a portfolio project, it highlights industry best practices in **data engineering** and **data analytics**.

---

## 🏛️ Data Architecture

The data architecture for this project follows the **Medallion Architecture**, organized into **Bronze**, **Silver**, and **Gold** layers:

1. **Bronze Layer** — Stores raw data exactly as received from the source systems. Data is ingested from CSV files into a SQL Server database with no transformations applied.
2. **Silver Layer** — Handles data cleansing, standardization, and normalization to prepare the data for analysis.
3. **Gold Layer** — Houses business-ready data modeled into a star schema, optimized for reporting and analytical queries.

> A detailed architecture diagram is available in the `docs/` folder.

---

## 📖 Project Overview

This project covers the full lifecycle of a modern analytics solution:

1. **Data Architecture** — Designing a modern data warehouse using the Medallion Architecture (Bronze, Silver, and Gold layers).
2. **ETL Pipelines** — Extracting, transforming, and loading data from the source systems into the warehouse.
3. **Data Modeling** — Building fact and dimension tables optimized for analytical queries.
4. **Analytics & Reporting** — Writing SQL-based reports to surface actionable business insights.

🎯 This repository is a useful reference for anyone looking to demonstrate skills in:
- SQL Development
- Data Architecture
- Data Engineering
- ETL Pipeline Development
- Data Modeling
- Data Analytics

---

## 🚀 Project Requirements

### Building the Data Warehouse (Data Engineering)

#### Objective
Develop a modern data warehouse using SQL Server to consolidate sales data, enabling analytical reporting and informed decision-making.

#### Specifications
- **Data Sources** — Import data from two source systems (ERP and CRM) provided as CSV files.
- **Data Quality** — Cleanse and resolve data quality issues prior to analysis.
- **Integration** — Combine both sources into a single, user-friendly data model designed for analytical queries.
- **Scope** — Focus on the latest dataset only; historization of data is not required.
- **Documentation** — Provide clear documentation of the data model to support both business stakeholders and analytics teams.

---

### BI: Analytics & Reporting (Data Analytics)

#### Objective
Develop SQL-based analytics to deliver detailed insights into:
- **Customer Behavior**
- **Product Performance**
- **Sales Trends**

These insights empower stakeholders with key business metrics, enabling strategic decision-making.

---

## 🛠️ Tech Stack & Tools

- **SQL Server** — Database engine hosting the data warehouse.
- **SQL Server Management Studio (SSMS)** — GUI for managing and querying the database.
- **CSV Datasets** — Raw source data from the ERP and CRM systems.
- **Draw.io** — For designing the data architecture, models, and flow diagrams.
- **Git & GitHub** — Version control and project collaboration.

---

## 📂 Repository Structure

```
data-warehouse-project/
│
├── datasets/                   # Raw ERP and CRM datasets (CSV files)
│
├── docs/                       # Project documentation and diagrams
│   ├── data_architecture.drawio    # Overall data architecture
│   ├── data_flow.drawio            # Data flow diagram
│   ├── data_models.drawio          # Star schema data models
│   ├── data_catalog.md             # Catalog of datasets and fields
│   └── naming_conventions.md       # Naming guidelines for tables and columns
│
├── scripts/                    # SQL scripts for ETL and transformations
│   ├── bronze/                     # Scripts for raw data ingestion
│   ├── silver/                     # Scripts for cleaning and transformations
│   └── gold/                       # Scripts for analytical (star schema) models
│
├── tests/                      # Test scripts and data quality checks
│
├── README.md                   # Project overview and instructions
├── LICENSE                     # License information
└── .gitignore                  # Files and folders ignored by Git
```

---

## ⚙️ Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/data-warehouse-project.git
   ```
2. **Set up the database** — Install SQL Server and SQL Server Management Studio (SSMS), then create the project database.
3. **Load the source data** — Place the ERP and CRM CSV files in the `datasets/` folder.
4. **Run the ETL scripts in order** — Execute the SQL scripts in `scripts/bronze/`, then `scripts/silver/`, then `scripts/gold/` to build out each layer of the warehouse.
5. **Explore the analytics** — Run the reporting queries to generate insights on customer behavior, product performance, and sales trends.


