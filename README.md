# Pizza-Sales-Data-Analytics---End-to-End-Azure-Data-Engineering-Production-level-project1
<div align="center">
  <a href="#">
    <img src="https://github.com/zBalachandar/Pizza-Sales-Data-Analytics---End-to-End-Azure-Data-Engineering-Production-level-project1/blob/main/Assets/Power%20BI%20report%20IMG.png" alt="Banner" width="720">
  </a>

  <div id="user-content-toc">
    <ul>
      <summary><h1 style="display: inline-block;">🔧 Analyzing Sales of Pizza sales Data🔌</h1></summary>
    </ul>
  </div>
  
  <p>On-prem DB to Azure Cloud Pipeline with Data Factory, Lake Storage, Spark, Databricks, Synapse, PowerBI</p>
</div>
<br>

## 📝 Table of Contents
1. [Project Overview](#introduction)
2. [Key Insights](#key-insights)
3. [Project Architecture](#project-architecture)  
  3.1. [Data Ingestion](#data-ingestion)  
  3.2. [Data Transformation](#data-transformation)  
  3.3. [Data Loading](#data-loading)  
  3.4. [Data Reporting](#data-reporting)
4. [Credits](#credits)
5. [Contact](#contact)

<a name="introduction"></a>
## 🔬 Project Overview 

This an end-to-end data engineering project on the Azure cloud. Where I did data ingestion from a on-premise SQL Server to Azure Data Lake using Data Factory to transformation using Databricks and Spark, loading to Synapse, and reporting using PowerBI. Also, I used Azure Active Directory (AAD) and Azure Key Vault for the data monitoring and governance purpose. 

### 💾 Dataset
Dataset link : https://drive.google.com/file/d/1i4aRieq_WDVJDGpqtZq8UW9CH8sCbaBd/view?pli=1

### 🎯 Project Goals

- Establish a connection between on-premise SQL server and Azure cloud.
- Ingest tables into the Azure Data Lake.
- Apply data cleaning and transformation using Azure Databricks.
- Utilize Azure Synapse Analytics for loading clean data.
- Create interactive data visualizations and reports with Microsoft Power BI.
- Implement Azure Active Directory (AAD) and Azure Key Vault for monitoring and governance.

<a name="key-insights"></a>
## 🕵️ Key Insights

- 💸 **Total Revenue by Product Category**
  - *Touring Bikes* is the top 1 category generating revenue with 32% followed by *Road Bikes* with 26% and *Mountain Bikes* with 24%.
 
- 🌍 **Sales by Country**
  - **N°1:** The United Kingdom (UK) have the most total sales with 278 and $572,000 of total revenue.
  - **N°2:** The United States of America (USA) is second with total sales with 264 and $383,810 of total revenue.

- 🚻 **Revenue by Gender**
  - 81% of the revenue is generated by Male customers
  - 19% of the revenue is generated by Female customers  

> This can be explained by males have more interest in doing outdoor activites with the different categories of Bikes than females.

<a name="project-architecture"></a>
## 📝 Project Architecture

You can find the detailed information on the diagram below:

![image](https://github.com/zBalachandar/Pizza-Sales-Data-Analytics---End-to-End-Azure-Data-Engineering-Production-level-project1/blob/e654d77b8eba8d60bc63aadd49832b0eefb9b910/Assets/Project%20Architecture-%20Sales%20data%20analytics.jpg)

<a name="data-ingestion"></a>
### 📤 Data Ingestion
- Connected the on-premise SQL Server with Azure using Microsoft Integration Runtime.

![image](https://github.com/Hamagistral/Azure-AW/assets/66017329/b57debac-28c2-4928-8640-676643e0177c)

- Setup the **Resource group** with needed services (Key Vault, Storage Account, Data Factory, Databricks, Synapse Analytics)

![ressource-group](https://github.com/Hamagistral/Azure-AW/assets/66017329/62990af9-db6e-4712-81bf-61420835bb99)

- Migrated the tables from on-premise SQL Server to Azure Data Lake Storage Gen2.

![image](https://github.com/Hamagistral/Azure-AW/assets/66017329/2b9855a9-9ad7-4ac3-8076-70762ef0f3bc)
![df-pipeline](https://github.com/Hamagistral/Azure-AW/assets/66017329/21ed74aa-8bf4-46c5-952c-4dc9f14dc9fb)

<a name="data-transformation"></a>
### ⚙️ Data Transformation
- Mounted Azure Blob Storage to Databricks to retrieve raw data from the Data Lake.
- Used Spark Cluster in Azure Databricks to clean and refine the raw data.
- Saved the cleaned data in a Delta format; optimized for further analysis.

![image](https://github.com/Hamagistral/Azure-AW/assets/66017329/11b7fb4e-0013-4a9f-a791-ab2a2789f774)

<a name="data-loading"></a>
### 📥 Data Loading
- Used Azure Synapse Analytics to load the refined data efficiently.
- Created SQL database and connected it to the data lake.

![synapse-pipeline](https://github.com/Hamagistral/Azure-AW/assets/66017329/99a8c7cd-1a6f-4ec9-b35d-2e171d3be87b)
![db-synapse](https://github.com/Hamagistral/Azure-AW/assets/66017329/b601eb00-efe1-44d9-8de6-8f001176d549)

<a name="data-reporting"></a>
### 📊 Data Reporting
- Connected Microsoft Power BI to Azure Synapse, and used the Views of the DB to create interactive and insightful data visualizations.

![PowerBI-dashboard](https://github.com/zBalachandar/Pizza-Sales-Data-Analytics---End-to-End-Azure-Data-Engineering-Production-level-project1/blob/e654d77b8eba8d60bc63aadd49832b0eefb9b910/Assets/Power%20BI%20report%20img%20Report%20with%20features.png)

### 🛠️ Technologies Used

- **Data Source**: SQL Server
- **Orchestration**: Azure Data Factory
- **Ingestion**: Azure Data Lake Gen2
- **Storage**: Azure Synapse Analytics
- **Authentication and Secrets Management**: Azure Active Directory and Azure Key Vault
- **Data Visualization**: PowerBI

<a name="credits"></a>
## 📋 Credits

- This Project is inspired by the video of the [YouTube Channel "Learn by doing it"](https://www.youtube.com/watch?v=pMqnvXgPKlI&list=PLOlK8ytA0MghGmAAT8W2u7VYmICdzeU5t&index=1&t=96s)  

<a name="contact"></a>
## 📨 Contact Me

[LinkedIn](https://www.linkedin.com/in/balachandars2022/) •
[Gmail](balachandar2014elu@gmail.com)  •
