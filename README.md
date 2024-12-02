## Azure Purview Data Governance Project

### Project Description
This repository contains the source code and documentation for a two-part series focusing on data governance using Azure Purview. This project is centered around the management and regulation of data across various environments, including on-premises, multi-cloud, and SaaS, through Azure Purview.

### Business Overview
Azure Purview provides a unified data governance solution that automates data discovery, sensitive data categorization, and data lineage creation. This allows for a holistic, up-to-date map of your data landscape, aiding data curators and consumers in managing and finding reliable data.

### Data Pipeline
The data pipeline includes steps from harvesting data to transforming it into a format ready for analysis. This project uses Azure services to handle data in real-time and batch processing modes, ensuring efficient data management across platforms.

### Agenda
Part 1: Data ingestion and preparation using Azure Logic Apps, Azure Storage Account, Azure Data Factory, and Azure SQL Databases.
Part 2: Data consumption and analysis utilizing the capabilities of Azure Purview.
Dataset Description
This project uses hospital data consisting of 30 unique fields, including:

### Hospital Name
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

### Key Steps

<img width="959" alt="1 Created Resource Group" src="https://github.com/user-attachments/assets/8fc31d1e-6fa2-4516-8e10-358056242e01">

1.Create a Resource Group: All related services are organized under a single resource group to facilitate better management and integration. This approach simplifies administration and enhances the ability to apply policies consistently across services.

<img width="959" alt="3 Create Storage" src="https://github.com/user-attachments/assets/3617cccb-2a63-49f5-96d4-c2ede601f76a">

2.Set Up Dropbox Account: Dropbox is used as an initial data repository where users can upload and update data. This step is crucial for gathering raw data before it's processed and transferred to Azure's ecosystem.


3.Establish Azure Storage Account: The data retrieved from Dropbox is stored in an Azure Storage Account. This service offers scalable and secure cloud storage for large amounts of data, which is essential for subsequent processing and analysis.

https://github.com/user-attachments/assets/6482625d-df4c-4fd4-ac29-5118b2ce5ed8

4.Develop Azure Logic App: An Azure Logic App is created to automate the process of data retrieval from Dropbox and its storage in Azure Blob Storage. This automation streamlines the workflow, reduces manual errors, and enhances efficiency.

<img width="959" alt="5 SQL Server" src="https://github.com/user-attachments/assets/281d26f0-4fdf-4777-bfed-ad0f547b7ff6">

5.Provision Azure SQL Database: Data is moved from Azure Blob Storage to an Azure SQL Database. This step is critical for transforming raw data into structured formats that are easier to query and analyze, enabling more sophisticated data processing and insights.

<img width="959" alt="9 Azure Data Factory" src="https://github.com/user-attachments/assets/6daaae98-e110-4bf7-92a6-3a7e044d6810">

6.Implement Azure Data Factory: An Azure Data Factory pipeline is set up to transfer data from Azure Storage to Azure SQL Database. This data pipeline is responsible for the seamless flow of data through different stages of processing, from ingestion to storage.

<img width="959" alt="11 Pipeline" src="https://github.com/user-attachments/assets/a182e59e-6a11-4deb-a1d8-48921c110614">

7.Building Data Pipeline: This involves creating a pipeline to transfer data from Azure Storage and sink it into Azure SQL. This pipeline not only moves the data but also can include steps for cleansing, transforming, and validating the data to ensure it's ready for analysis.
   
<img width="959" alt="12 PruviewAccountCreating" src="https://github.com/user-attachments/assets/7193ac87-7565-4e7f-a848-cb0e6e24e7c3">

8.Configure Azure Purview: Azure Purview is integrated to govern the data landscape. It helps in mapping, cataloging, and analyzing data across various Azure services, providing a unified view of data governance and compliance.

<img width="959" alt="13 Setting up Sources in purview" src="https://github.com/user-attachments/assets/e1343391-be54-4143-9b8e-8534ed7246bf">

9.Connecting Sources with Azure Purview: Once the Azure Purview account is set up, it is connected with Azure SQL to begin scanning and cataloging data assets. This connection is essential for Azure Purview to access and manage the metadata and data assets stored in Azure SQL.

<img width="959" alt="14  Scan Complete" src="https://github.com/user-attachments/assets/70053946-fae7-4391-9bed-76b1aba710af">

10.Scan Complete and Asset Management: After the scan is complete, data and metadata are visible within Azure Purview, allowing users to manage and analyze various data assets easily. The integration with Azure Key Vault ensures that all connections and sensitive data are secured.

<img width="959" alt="15  Assets" src="https://github.com/user-attachments/assets/6670961a-fd78-4591-99e7-7a07c551d737">
11.View and Manage Assets in Azure Purview: Once the data assets are scanned and cataloged in Azure Purview, users can view both data and metadata. This visibility is crucial as it allows users to understand not just the raw data but also its context and structure. Metadata includes information about data origin, format, and relationships with other data, which are essential for comprehensive data governance. This step enhances data discoverability and governance by providing a clear and organized view of all data assets within the Azure ecosystem, making it easier for data curators and consumers to manage and utilize their data effectively.

#### Using Azure Purview
Azure Purview is instrumental in scanning and categorizing data assets across your estate. It constructs a comprehensive data map that supports data discovery, access management, and analysis.
