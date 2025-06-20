# 🌐 Automated Health Data Pipeline with CI/CD

This project demonstrates a real-time, production-ready **Data Engineering Pipeline** using Azure services and CI/CD automation through GitHub Actions. It integrates ingestion, transformation, analysis, visualization, and automated deployment across environments

---

## 🔧 Solution Architecture

![Solution Architecture](https://github.com/AnmolHajnale/major-Project-cicd/blob/main/Architecture.png)

---

## 📌 Key Features

- Ingests **COVID-19 data (via HTTP)** and **Population Data (via Blob Storage)**
- Stores data in **Azure Data Lake Gen2** (raw + processed layers)
- Transforms and analyzes using **Azure Data Factory** and **Azure Databricks**
- Loads data into **Azure SQL Database** for reporting
- Visualizes insights using **Power BI**
- ML-ready data also stored for **ML model access**
- Fully automated CI/CD pipeline using **GitHub Actions**
- Implements **Scheduled + Tumbling Window triggers**

---

## 🔄 CI/CD with GitHub Actions

- Code is stored in GitHub
- On commit, GitHub Actions:
  - Builds ARM templates
  - Packages artifacts
  - Deploys to **ADF Test** and **ADF Prod**
- Pure GitHub-based CI/CD (no Azure DevOps)

---

## 🛠️ Tech Stack

| Tool/Service              | Purpose                                   |
|---------------------------|--------------------------------------------|
| Azure Data Factory        | ETL pipelines and no-code transformations |
| Azure Databricks          | Scalable data transformation & analytics  |
| Azure SQL Database        | Data storage & analytics                  |
| Azure Data Lake Gen2      | Raw & processed data storage              |
| Power BI                  | Dashboards and visual analytics           |
| GitHub + GitHub Actions   | Version control and CI/CD automation      |
| ARM Templates             | Infrastructure as Code (IaC)              |
| ADF Triggers              | Scheduled and tumbling window automation  |

---

## 📁 Repository Structure

