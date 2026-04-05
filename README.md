# SAP Access Tracker

A security analytics tool designed to monitor and manage user access 
within SAP environments, ensuring compliance and minimizing security risks 
through automated data pipelines and interactive dashboards.

> ⚠️ **Note**: This project was developed during a private company 
> internship. No proprietary code or sensitive data is shared in this 
> repository. This README serves as a documentation of the work done 
> and the technologies used.

## 📌 Overview
Organizations running SAP systems face the challenge of ensuring that 
users have only the permissions they need — nothing more, nothing less. 
SAP Access Tracker addresses this by providing a full pipeline from data 
extraction to real-time visual reporting, enabling security teams to 
monitor access patterns, detect anomalies, and maintain compliance.

## 🔄 Pipeline Architecture
SAP System → Python Extraction Script → Atlas Cloud (MongoDB) → Power BI (via ODBC) → Dashboard & KPIs

## ⚙️ How It Works

**1. Data Extraction**
Pulls transaction-level data from SAP systems daily, capturing:
- Transaction logs (TCode and Report types)
- User account information
- Entity-level access details
- Entry-specific metadata for audit purposes

**2. Secure Cloud Storage**
Extracted data is stored in **Atlas Cloud (MongoDB)**, ensuring 
centralized, secure, and scalable storage with data integrity controls.

**3. Data Cleaning & Transformation (Power BI)**
Connected via ODBC driver, the raw data undergoes:
- Column type standardization
- Removal of redundant fields
- Error handling and null value management
- Sorting and structuring for analytical readiness

**4. Visualization & KPI Reporting**
Interactive Power BI dashboards provide:
- Granular transaction tables with dynamic filters
- KPIs tracking access patterns and permission compliance
- Anomaly indicators for quick security response

## 🤖 Automation
The entire pipeline runs automatically on a daily schedule:
- **Extraction**: Triggered by **Windows Task Scheduler**
- **Dashboard Refresh**: Handled by **Power BI Service Gateway**

This ensures security teams always have access to up-to-date insights 
without any manual intervention.

## 🛠️ Tech Stack
Python · MongoDB Atlas · Power BI · ODBC · Windows Task Scheduler · SAP

## ✨ Key Features
- 🔐 Granular user access monitoring at account and entity level
- ☁️ Secure centralized cloud storage
- 🔄 Fully automated daily pipeline
- 📊 Interactive dashboards with customizable filters
- 📈 Real-time KPIs for compliance tracking
- 🧹 Automated data cleaning and transformation
