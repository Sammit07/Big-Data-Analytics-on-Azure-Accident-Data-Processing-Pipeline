# 📊 Big Data Analytics on Azure – Accident Data Processing Pipeline

The **Accident Data Processing Pipeline** is a big data project built on **Microsoft Azure** using **HDInsight, Hive, Sqoop, Data Lake Gen2, and Azure SQL Database**.  
It demonstrates the end-to-end workflow of ingesting, transforming, analyzing, and loading accident data using **cloud-based big data tools**. 

---

## 📌 Features

- ☁️ **Cloud-Native Data Lake**: Data stored in **Azure Data Lake Storage Gen2**.  
- 🔑 **Identity & Access**: Used **Azure Active Directory Managed Identity** for secure access to storage.  
- 🗃️ **Structured Data Processing**: Transformed raw CSV accident data into Hive external tables.  
- 📊 **Analytics with Hive**: Ran HiveQL queries to calculate accident statistics by day of the week.  
- 🔄 **ETL Workflow**: Exported processed data from Hadoop to **Azure SQL Database** using **Sqoop**.  
- 🛠️ **Hadoop Ecosystem**: Leveraged **HDInsight cluster** for distributed data processing.  

---

## 🌟 Project Overview

The project was implemented step by step:

### 🔹 Step 1: Create User-Managed Identity
- **Tool**: Azure Active Directory  
- **Purpose**: Allows Hadoop cluster to securely access Data Lake Gen2.  

### 🔹 Step 2: Create Data Lake Gen2 Account
- **Tool**: Azure Portal / CLI  
- **Purpose**: Store raw accident datasets.  

### 🔹 Step 3: Configure Permissions
- **Tool**: Azure Portal / CLI  
- **Purpose**: Assign permissions for managed identity to access Data Lake.  

### 🔹 Step 4: Provision SQL Database
- **Tool**: Azure SQL Database  
- **Purpose**: Store transformed accident data for downstream use.  

### 🔹 Step 5: Create Hadoop Cluster
- **Tool**: Azure HDInsight  
- **Purpose**: Distributed processing of accident data using Hive & Sqoop.  

### 🔹 Step 6: Upload Data & Scripts
- **Tool**: Azure Data Lake Gen2  
- **Purpose**: Upload raw CSV data and HiveQL staging scripts.  

### 🔹 Step 7: Transform Data with Hive
- **Tool**: Apache Hive on HDInsight  
- **Purpose**: Create external Hive tables, clean data, and calculate accident stats.  

### 🔹 Step 8: Export Data with Sqoop
- **Tool**: Apache Sqoop  
- **Purpose**: Load processed Hive data into Azure SQL Database.  

---

## 🏗️ Architecture

<img width="1556" height="582" alt="image" src="https://github.com/user-attachments/assets/f09e0cd4-3d7d-4105-b474-7fb63f55394e" />



---

## 🛠️ Tech Stack

- **Cloud Platform**: Microsoft Azure  
- **Big Data Tools**: HDInsight (Hadoop Cluster), Hive, Sqoop  
- **Storage**: Azure Data Lake Storage Gen2  
- **Database**: Azure SQL Database  
- **Security**: Azure Active Directory Managed Identity  
- **Languages & Tools**: HiveQL, SQL, Hadoop ecosystem  

---

## 🔒 Security Best Practices

- Used **Managed Identity** to avoid hardcoding credentials.  
- Granted **least-privilege access** to storage and database.  
- Data stored in **Azure Data Lake Gen2** with role-based permissions.  

---

## 📊 Key Insights

- The HiveQL query calculated the **total number of vehicles involved in accidents per weekday**.  
- 🚗 **Saturday recorded the highest number of accidents with 647,338 vehicles involved**.  

---

## 🚀 Future Enhancements

- Automate the ETL pipeline with **Azure Data Factory**.  
- Use **Power BI** dashboards for interactive accident analysis.  
- Apply **machine learning models** for accident prediction and trend analysis.  
- Implement **data partitioning** in Hive for faster query performance.  
