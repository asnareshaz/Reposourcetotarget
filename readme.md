Initialized by Azure Data Factory!
**Introduction**
________________________________________
This project is a POC for testing the functionalities of Azure Data Factory in order to adapt with the requirements from the problem statement.

**What is Azure Data Factory?**

Azure Data Factory is a cloud-based data integration service for creating ETL (Extract, Transform and Load) and ETL pipelines. It allows users to create data processing workflows in the cloud, either through a graphical interface or by writing code, for orchestrating and automating data movement and data transformation. It is possible to build complex ETL processes that transform data visually with data flows or by using compute services such as Azure HDInsight Hadoop, Azure Databricks, and Azure SQL Database.

**Requirement**

• Create, run and manage pipelines for data transfer between Amazon S3 & Azure Blob Storage.
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
2.	On the Azure Windows, some raw data were copied into this Budget_Lines table to simulate the scenario of raw data at the MySql . We use azcopy tool to perform the data transfer from MySql to Azure Blob.
3.	Once we have the raw data on Azure, we create different pipelines to transfer these data to test container on Azure Blob Storage.
4.	
**Build and Test**

1.	Login to amazon console and create required bucket under S3.

![image](https://user-images.githubusercontent.com/94681830/143837435-6195c74f-daa0-4935-8346-73438619aed2.png)

a.upload external data in S3 buckets.

![image](https://user-images.githubusercontent.com/94681830/143837575-7b5aaf0b-7389-4208-b026-6a7a959af7c6.png)

b. create new policy under IAM for  S3 as new user.

![image](https://user-images.githubusercontent.com/94681830/143837741-ee289c86-67ec-43a3-89df-1f81ccaed990.png)

![image](https://user-images.githubusercontent.com/94681830/143837817-0b1df77d-5d2d-4542-9468-1b8137bd5050.png)

![image](https://user-images.githubusercontent.com/94681830/143837906-c9088f1c-f4e9-43cf-89c8-a86cba1fbf0c.png)

![image](https://user-images.githubusercontent.com/94681830/143838140-57a6e611-dd92-481f-abee-e612cf6bea01.png)

![image](https://user-images.githubusercontent.com/94681830/143838196-5d79a508-5634-4843-b224-5856f3b079ef.png)

![image](https://user-images.githubusercontent.com/94681830/143838756-13c2b074-fb77-47fc-b012-be8bfc8c8ced.png)

c. attach S3 polcy to the new users.

2.Navigate to Azure Data Factory portal, This Azure Data Factory is running on the Windows Server. Click on Author & Monitor to open the editor mode of Azure Data Factory.

![image](https://user-images.githubusercontent.com/94681830/143839672-417833fa-3083-427b-94c5-17d327537682.png)

3.Click on Azure Data Factory Studio.

![image](https://user-images.githubusercontent.com/94681830/143839749-f93456b9-66ac-47e7-a25e-5f44d97bbd75.png)

4.Create a new dataset for AWS S3.

![image](https://user-images.githubusercontent.com/94681830/143839887-2e76f943-a1cc-4293-9e2e-c1cd72aaa31f.png)

![image](https://user-images.githubusercontent.com/94681830/143840069-b211174a-6695-46f8-b449-0a6f35d40f62.png)

5.Create a new datset for Blob 

![image](https://user-images.githubusercontent.com/94681830/143840487-cafedd4e-e1ec-42cf-94f1-4d3e7c084b79.png)

![image](https://user-images.githubusercontent.com/94681830/143840594-0513dc17-12cd-4ea2-b035-89e21ad316f9.png)

6.Create a new pipeline for copying the data between AWS S3 to Blob.

![image](https://user-images.githubusercontent.com/94681830/143840764-b3afda62-b349-4148-9a44-5c3dd243b0e7.png)


