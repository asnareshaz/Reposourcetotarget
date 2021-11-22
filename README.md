Initialized by Azure Data Factory!

**Introduction**
__________________________________________________________________________________________________________________________________________________
This project is a POC for testing the functionalities of Azure Data Factory in order to adapt with the requirements from the problem statement.

**What is Azure Data Factory?**

Azure Data Factory is a cloud-based data integration service for creating ETL (Extract, Transform and Load) and ETL pipelines. It allows users to create data processing workflows in the cloud, either through a graphical interface or by writing code, for orchestrating and automating data movement and data transformation. It is possible to build complex ETL processes that transform data visually with data flows or by using compute services such as Azure HDInsight Hadoop, Azure Databricks, and Azure SQL Database.

**Requirement**

•	Create, run and manage pipelines for data transfer between Azure blob storage & Azure Blob Storage.

1.	Line Number
2.	Budget Code
3.	PurchaseOrg
4.	PurchaseGroup
5.	CompanyCode
6.	CostCenter
7.	GeneralLedger
8.	WBSElement
9.	Asset
10.	SubNumber
11.	InternalOrder
12.	ProjectNumber
13.	Rank
14.	Budget Check Disabled

•	Automation of the pipeline to be able to check the state of the last pipeline run

**Getting Started**

1.	Required to have Azure with Windows Server to host Azure Data Factory.
2.	On the Azure Windows, some raw data were copied into this Flatfiles to simulate the scenario of raw data at the edge machine. We use azcopy tool to perform the data transfer     from Blob storage to Azure.
3.	Once we have the raw data on Azure, we create different pipelines to transfer these data to test container on Azure Blob Storage.
![image](https://user-images.githubusercontent.com/94681830/142822989-3fb03564-877b-4ece-a86e-e217572ec472.png)
4.  raw data were copied from local to New1117 container .
![image](https://user-images.githubusercontent.com/94681830/142823319-e40f536b-4a89-4373-9c39-8d9a842f3a94.png)








