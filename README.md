# Data-Driven Policy Modeling for COVID-19

A comprehensive data science project analyzing COVID-19 policies to identify the optimal balance between public health effectiveness and minimal economic restrictions.

## Project Overview

This project supports government leaders in making data-driven decisions for COVID-19 policy management. Using real-world international data, we developed a model to maintain:

- COVID-19 death growth rate below **1%**
- New case growth rate below **3%**
- 30-day rolling average monitoring

## Data Architecture

Our data architecture is built on modern cloud tools:

- **Extract & Load**  
  - Data sourced from:
    - Azure SQL
    - VM SQL Server
    - Cosmos DB

- **Transform**  
  - Processing via **Azure Data Factory**

- **Load**  
  - Storage in **Azure Synapse Analytics** using a Galaxy Schema

- **Visualize**  
  - Interactive dashboards in **Power BI**


## Data-Driven-Policy-Modeling-for-COVID-19 Structure

- `Azure Data Factory/`     - Data pipeline configurations
- `arm_template/`          - Azure Resource Manager templates
- `Data Model.png`         - Database schema diagram
- `Executive Summary.pdf`  - Project summary and findings
- `Final Presentation.mp4` - Video presentation
- `PowerBI Analysis.pbix`  - Power BI dashboard
- `Presentation.pdf`       - Detailed project presentation
- `Schema.png`            - Galaxy schema visualization

## Setup Steps
- **Deploy Azure Resources:**
  - bash# Use the ARM template in arm_template/ folder    
  - az deployment group create --resource-group your-rg --template-file template.json     

- **Configure Data Factory:**

  - Import pipelines from Azure Data Factory folder    
  - Set up data source connections
  - Configure transformation logic


- **Load Data:**

  - Execute data pipelines to populate the data warehouse
  - Verify data quality and completeness


- **Open Power BI Dashboard:**

  - Open `PowerBI Analysis.pbix`
  - Refresh data connections
  - Explore interactive visualizations
