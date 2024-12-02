Azure Purview Data Governance Project
Project Description
This repository contains the source code and documentation for a two-part series focusing on data governance using Azure Purview. This project is centered around the management and regulation of data across various environments, including on-premises, multi-cloud, and SaaS, through Azure Purview.

Business Overview
Azure Purview provides a unified data governance solution that automates data discovery, sensitive data categorization, and data lineage creation. This allows for a holistic, up-to-date map of your data landscape, aiding data curators and consumers in managing and finding reliable data.

Data Pipeline
The data pipeline includes steps from harvesting data to transforming it into a format ready for analysis. This project uses Azure services to handle data in real-time and batch processing modes, ensuring efficient data management across platforms.

Agenda
Part 1: Data ingestion and preparation using Azure Logic Apps, Azure Storage Account, Azure Data Factory, and Azure SQL Databases.
Part 2: Data consumption and analysis utilizing the capabilities of Azure Purview.
Dataset Description
This project uses hospital data consisting of 30 unique fields, including:

Hospital Name
Address
Hospital Type
Mortality National Comparison
Patient Experience National Comparison Footnote
Hospital Overall Rating
Criteria for Meaningful Use of EHRs
Tech Stack
Azure Logic Apps
Azure Storage Account
Azure Data Factory
Azure SQL Databases
DBeaver
Azure Purview
Key Steps
Create a Resource Group: Organize all related services under a single resource group for better management.
Set Up Dropbox Account: Use Dropbox for initial data storage and updates.
Establish Azure Storage Account: Store data retrieved from Dropbox.
Develop Azure Logic App: Automate data retrieval from Dropbox to Azure Blob Storage.
Provision Azure SQL Database: Move data from Azure Blob Storage to SQL Database.
Implement Azure Data Factory: Create a data pipeline for transferring data from Azure Storage to Azure SQL.
Configure Azure Purview: Integrate Azure Purview for data governance and map creation.
Link Data Sources: Use Azure Key Vault to secure connections between Azure Purview and SQL Database.
Using Azure Purview
Azure Purview is instrumental in scanning and categorizing data assets across your estate. It constructs a comprehensive data map that supports data discovery, access management, and analysis.
