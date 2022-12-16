# Game Sales-Analysis-MSBI

![Report](https://user-images.githubusercontent.com/17761176/207992014-38c9bd4e-581b-477d-8786-990324ad1bf1.png)

An SSIS, SSAS and SSRS Game sales analysis project.

SSIS Steps:

Given an excel file with game sales data from here 
https://www.kaggle.com/datasets/gregorut/videogamesales

Step 1.1. Staging:

Import the excel sheet into sql to create a staging table.

Step 1.2. Creating a Datawarehouse and ETL process

Create a ssis(intergration services project) project to create a datawarehouse as well as extract transform and load the data from the staging table into the newly created datawarehouse

Create a datawarehouse with fact tables and dimensions using this script:

[GameSalesDW.txt](https://github.com/mandlenkosi-Tshabalala/Sales-Analysis-MSBI/files/10241472/GameSalesDW.txt)

ETL script:

[ETLDW.txt](https://github.com/mandlenkosi-Tshabalala/Sales-Analysis-MSBI/files/10241489/ETLDW.txt)

![ETL](https://user-images.githubusercontent.com/17761176/207989946-ea66c4f5-227a-4c4b-84f4-4d91fefc4f66.png)




SSAS steps:

Step 2.1. Create an ssas(analysis services multidimensional and data mining project) project.

Step 2.2 Create a datasource pointing to the datawarehouse created as well as a datasource view. Create a new cube selecting the measures and dimensions as shown in the following diagram:

![Cube](https://user-images.githubusercontent.com/17761176/207990890-70cc7144-a56d-4e54-9c3a-1e1b57ea32e7.png)

Step 2.3. Build deploy and process the project.


SSRS steps.

Step 3.1 Create a new ssrs(reporting server project) project.

Step 3.2 Create a new report and dataset using the query builder:

![QueryDesigning](https://user-images.githubusercontent.com/17761176/207991621-6bab0589-e401-4c4b-8e02-4aad782c9adf.png)

Step 3.3 Create a report using the report builder then publish it.

![Report](https://user-images.githubusercontent.com/17761176/207991963-3c89684f-8600-4589-bd07-7add5810b787.png)

