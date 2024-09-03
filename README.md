# Summer-internship
# SAP Access Tracker

SAP Access Tracker is a robust security tool designed for organizations to effectively monitor and manage client access within SAP systems. By extracting detailed transaction data, securely storing it in Atlas Cloud, cleaning and transforming it in Power BI, and providing comprehensive visualizations and KPIs, SAP Access Tracker helps maintain a secure SAP environment while ensuring access compliance.

## Table of Contents

- [Introduction](#introduction)
- [Data Extraction, Storage, Cleaning, and Visualization](#data-extraction-storage-cleaning-and-visualization)
- [Features](#features)
- [Automation](#automation)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

SAP Access Tracker is essential for organizations looking to enforce robust access management practices within SAP environments. It tracks user access on a per-account or per-entity basis, ensuring that each client has the necessary permissions without exceeding what's required—minimizing security risks. The tool is versatile, handling both TCode and report transactions to provide a comprehensive security overview.

## Data Extraction, Storage, Cleaning, and Visualization

SAP Access Tracker follows a rigorous process to ensure data integrity, security, and usability:

Data Extraction: Extracts a comprehensive dataset containing:

SAP Transaction Entries: A detailed log of every transaction.
Account Information: Identifies the user account that performed each transaction.
Entity Details: Specifies the entity to which each account belongs.
Transaction Type: Classifies each transaction as either TCode or report.
Entry Details: Provides specifics for each transaction, aiding in auditing and security assessments.
Secure Storage in Atlas Cloud: The extracted data is securely stored in Atlas Cloud, a robust cloud platform that ensures data privacy and integrity. This centralized repository facilitates effective access management and auditing.

Data Cleaning and Transformation in Power BI: Using an ODBC driver connection, the data is sent to Power BI where it undergoes thorough cleaning and preparation, including:

Changing column types to ensure data consistency.
Deleting unnecessary data to enhance clarity and focus.
Managing errors and resolving inconsistencies.
Replacing missing values for completeness.
Sorting and organizing the data for efficient analysis.
Data Visualization and KPI Reporting: Post-cleaning, the data is visualized in Power BI through:

Transaction Tables: Detailed tables for each type of transaction with filters to allow users to view data with specific parameters.
Key Performance Indicators (KPIs): Customized KPIs that provide insights into security and access patterns, enabling quick and informed decision-making.

##Features
Comprehensive Access Tracking: Monitors user access within SAP systems on a granular level.
Efficient Permission Management: Ensures that users have only the necessary permissions, minimizing security risks.
Proactive Security Alerts: Identifies and alerts for access that exceeds defined thresholds.
Detailed Data Logs: Extracts and logs data necessary for thorough security audits.
Secure Cloud Storage: Utilizes Atlas Cloud to securely store extracted data.
Advanced Data Cleaning and Transformation: Cleans and transforms data in Power BI, enhancing its quality and usability.
Interactive Visualizations and Reports: Provides dynamic tables, visualizations, and KPIs for deep analysis.

## Automation
The entire process is automated to run daily using Windows Task Scheduler. This automation ensures that data remains current, providing up-to-date insights and maintaining a secure SAP environment. The daily updates help organizations quickly identify and respond to any potential security threats.

## Contributing
We welcome contributions to the SAP Access Tracker project! To contribute:

Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes.
Commit your changes (git commit -m 'Add a new feature').
Push to the branch (git push origin feature-branch).
Open a Pull Request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contact
For more information or support, please contact:
Your Name - your-email@example.com
