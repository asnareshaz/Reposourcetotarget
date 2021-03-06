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

**Build and Test**
1.  Navigate to Azure Data Factory portal, This Azure Data Factory is running on the Windows Server. Click on Author & Monitor to open the editor mode of Azure Data Factory. 
![image](https://user-images.githubusercontent.com/94681830/142825597-fee510eb-3b9b-4517-8958-104da3fafb63.png)
2.  New containers created under storage account
![image](https://user-images.githubusercontent.com/94681830/142822989-3fb03564-877b-4ece-a86e-e217572ec472.png)
3.  Budget Lines data were copied from local to New1117 container .
![image](https://user-images.githubusercontent.com/94681830/142823319-e40f536b-4a89-4373-9c39-8d9a842f3a94.png)
4.  Budget Lines empty file were created in New1119 container.
![image](https://user-images.githubusercontent.com/94681830/142829553-1697e948-b2e0-46c5-9edb-ab5186ac077a.png)
![image](https://user-images.githubusercontent.com/94681830/142824437-4c2d6800-d207-48a4-a061-0febe44cb1e9.png)
4.  Click on Azure Data Factory Studio.
![image](https://user-images.githubusercontent.com/94681830/142826301-ca498b07-0525-4295-a629-f7ed64728776.png)
4.  Under the left menu Factory Resources is where you can find all the available pipelines,datasets & activities.
![image](https://user-images.githubusercontent.com/94681830/142826687-824e5639-6c23-4cbf-8adc-c89ef11f5f67.png)
5.  The Pipeline has the following workflow
![image](https://user-images.githubusercontent.com/94681830/142827506-276b2de2-4f42-4a0a-a3ed-798a74fc5db9.png)
6.  Data were copied into other file
![image](https://user-images.githubusercontent.com/94681830/142829447-6254cb70-0ccf-4526-932b-b050eef44422.png)









