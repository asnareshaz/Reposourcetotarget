Initialized by Azure Data Factory!

**Introduction**
________________________________________
This project is a POC for testing the functionalities of Azure Data Factory in order to adapt with the requirements from the problem statement.

**What is Azure Data Factory?**
Azure Data Factory is a cloud-based data integration service for creating ETL (Extract, Transform and Load) and ETL pipelines. It allows users to create data processing workflows in the cloud, either through a graphical interface or by writing code, for orchestrating and automating data movement and data transformation. It is possible to build complex ETL processes that transform data visually with data flows or by using compute services such as Azure HDInsight Hadoop, Azure Databricks, and Azure SQL Database.

**Requirement**
• Create, run and manage pipelines for data transfer between MySql & Azure Blob Storage.
1.	Line_Number
2.	Budget_Code
3.	PurchaseOrg
4.	PurchaseGroup
5.	CompanyCode
6.	Cost_Center
7.	GeneralLedger
8.	WBSElement
9.	Asset
10.	SubNumber
11.	InternalOrder
12.	ProjectNumber
13.	Rank_List
14.	Budget_Check_Disabled
• Automation of the pipeline to be able to check the state of the last pipeline run

**Getting Started**
1.	Required to have  MySql to host Azure Data Factory.
2.	On the Azure Windows, some raw data were copied into this Budget_Lines table to simulate the scenario of raw data at the MySql .
3.	We use azcopy tool to perform the data transfer from MySql to Azure Blob.
4.	Once we have the raw data on Azure, we create different pipelines to transfer these data to test container on Azure Blob Storage.

**Build and Test**
1.	Login to MySql and create required table in database
![image](https://user-images.githubusercontent.com/94681830/143833431-33544836-8bef-4ef8-b682-0938c9d9eaf7.png)

2.Navigate to Azure Data Factory portal, This Azure Data Factory is running on the Windows Server. Click on Author & Monitor to open the editor mode of Azure Data Factory.

![image](https://user-images.githubusercontent.com/94681830/143833750-c1d66b4c-92b6-4b28-a07c-594b5074f41c.png)

3.Click on Azure Data Factory Studio.
4.	
![image](https://user-images.githubusercontent.com/94681830/143834023-69c4e219-960d-4516-a3f5-6c67a9c3ee9f.png)

4.Under the left menu Factory Resources is where you can find all the available pipelines,datasets & activities.

![image](https://user-images.githubusercontent.com/94681830/143834448-e9698acb-56ca-4fc9-9d9a-c469b9298d02.png)
5.The Pipeline has the following workflow
6.	
![image](https://user-images.githubusercontent.com/94681830/143834530-ae07274a-2a76-4dc2-a5c4-2953a0c81f1d.png)
6.	Two datasets we have and which defines  MySql & Blob details.
a.	Dataset details using Linked service for MySql

![image](https://user-images.githubusercontent.com/94681830/143834629-5e1b721a-1ee8-44f5-9fc0-77579fad543f.png)

![image](https://user-images.githubusercontent.com/94681830/143834808-c9f9a9b1-01c9-4043-ac70-ae98abc83683.png)

b.Selfhosted integration runtime details.

![image](https://user-images.githubusercontent.com/94681830/143834902-a4723be9-177c-4ed8-9833-e6f417712387.png)

c.Click here to install self hosted integration in windows.

![image](https://user-images.githubusercontent.com/94681830/143834989-7c7a3ec7-5656-4424-a9da-fd4cd5c2cb04.png)
d.Dataset details using Linked service for Blob

![image](https://user-images.githubusercontent.com/94681830/143835087-6dbcb27e-e562-4d08-a211-99ba8cf24857.png)
![image](https://user-images.githubusercontent.com/94681830/143835170-c0183986-3320-4993-9cb1-775f29cf3764.png)

e.Pipeline were executed and data got transfered.

![image](https://user-images.githubusercontent.com/94681830/143835387-78a930b6-8752-466b-b611-303105b333d0.png)
![image](https://user-images.githubusercontent.com/94681830/143835444-0bb2dbe0-3a6d-443a-8e7b-d9d43fe67075.png)
![image](https://user-images.githubusercontent.com/94681830/143835489-021d3c3e-0324-4575-8b3c-c7e4e44dc7b5.png)






