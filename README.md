# 🌐 Automated Health Data Pipeline with ADF and CI/CD

This project demonstrates an end-to-end real-time data pipeline using **Azure Data Factory (ADF)**, **Azure Data Lake Storage Gen2**, **Azure SQL Database**, **Power BI**, and **CI/CD automation** using **GitHub Actions**.

---

## 🔧 Solution Architecture

![Solution Architecture](https://raw.githubusercontent.com/AnmolHajnale/major-Project-cicd/main/Screenshot%202025-01-22%20052953.png)

### 🔹 Components:
- **Data Sources**: 
  - ECDC COVID-19 Data (via HTTP connector)
  - Population data (Azure Blob Storage)
- **Ingestion & Transformation**:
  - Azure Data Factory pipelines to extract, load, and transform data
  - Stored in Azure Data Lake Gen2
- **Data Analysis & Storage**:
  - Data is transformed and moved to Azure SQL Database
- **Publishing & Reporting**:
  - Data is published using ADF pipelines and visualized in Power BI
- **ML Integration** (optional):
  - Data available for ML model training/serving via Azure Data Lake Gen2

---

## 🔄 CI/CD with GitHub Actions

![CI/CD Architecture](https://raw.githubusercontent.com/AnmolHajnale/major-Project-cicd/main/Screenshot%202025-01-22%20053157.png)

- **ADF Dev**: You develop and test pipelines in the Dev environment.
- **GitHub**: All ADF code (pipelines, datasets, triggers, linked services) is stored in Git and versioned.
- **CI/CD Workflow**:
  - On commit: A GitHub Action builds the ARM templates.
  - Artifacts are packaged.
  - GitHub Actions then deploys to **ADF Test**, and on approval to **ADF Prod**.

---

## 🛠️ Tech Stack

| Tool/Service              | Purpose                          |
|---------------------------|----------------------------------|
| Azure Data Factory        | ETL pipelines                    |
| Azure SQL Database        | Data storage & analytics         |
| Azure Data Lake Gen2      | Raw & processed data storage     |
| Power BI                  | Dashboards and visual analytics  |
| GitHub Actions            | CI/CD automation                 |
| ARM Templates             | Infrastructure as Code (IaC)     |

---

## 📁 Repository Structure

