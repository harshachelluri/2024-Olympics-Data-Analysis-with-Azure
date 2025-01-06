# **2024 Olympics Data Analysis with Azure**

## Project Overview

This project performs a comprehensive analysis of the 2024 Olympics data, leveraging the capabilities of **Azure** for cloud-based data storage, processing, and analysis. The analysis covers athlete demographics, medal distribution, gender representation, and performance across various sports and disciplines. The project uses **Azure Data Services** for storage, **Azure Data Factory (ADF)** for data pipeline orchestration, and **Power BI** for visualization and reporting.

## Datasets

The following datasets are included in the analysis:

- **Athletes_Data.csv**: Contains information about the athletes, including their names, countries, gender, and date of birth.
- **Coaches_dATA.csv**: Contains data about the coaches, including their names, countries, and sports.
- **Medal_Data.csv**: Contains medal data, categorized by gender (male, female, mixed) and country.
- **Team_Data.csv**: Contains data on the teams, including the events and disciplines they participated in.
- **Total_Medals.csv**: Contains the total number of medals (gold, silver, bronze) won by each country.
- **mfm_medal.csv**: Includes the number of medals won by male, female, and mixed teams.

## Technologies Used

- **Azure Data Services**: Used for cloud-based data storage and management.
  - **Azure Blob Storage (ABS)**: Stores datasets and processed data.
  - **Azure SQL Database**: Stores cleaned and aggregated data for further analysis.
- **Azure Data Factory (ADF)**: Orchestrates data pipelines for data ingestion, transformation, and movement between Azure Blob Storage and Azure SQL Database.
- **Power BI**: Used for creating dashboards and visualizing insights.
- **Python**: For data manipulation, analysis, and automation of workflows.

## Key Insights & Analysis

### 1. **Athletes Representing the USA**
   - Filters and displays athletes representing "Armenia" (code needs adjustment to filter for "USA").

### 2. **Total Medals Won by Gender**
   - Summarizes the total medals (gold, silver, bronze) won by male, female, and mixed teams.

### 3. **Total Medals Won by Each Country**
   - Breaks down the gold, silver, and bronze medals won by each country.

### 4. **Medals Awarded by Sport**
   - Counts the number of medals awarded in each sport.

### 5. **Average Age of Athletes**
   - Calculates the average age of athletes participating in the 2024 Olympics.

### 6. **Average Age by Gender**
   - Computes the average age of male and female athletes separately.

### 7. **Gender Distribution of Athletes**
   - Displays the number of male and female athletes.

### 8. **Event Count in the 2024 Olympics**
   - Counts the number of events participated in by different teams.

### 9. **Athletes' Distribution Across Genders and Disciplines**
   - Groups athletes by gender and discipline to show their distribution.

## Azure-Based Setup and Requirements

### Azure Resources

1. **Azure Blob Storage (ABS)**: Store raw datasets and processed files.
   - Create a storage account and container to upload the datasets.
   
2. **Azure Data Factory (ADF)**: 
   - Create ADF pipelines to automate the ingestion, transformation, and movement of data between Azure Blob Storage and Azure SQL Database.
   - Set up scheduled triggers to automate the data pipeline and processing.

3. **Azure SQL Database**:
   - Store cleaned and aggregated data for analysis, reporting, and visualization in **Power BI**.

4. **Power BI**:
   - Visualize the cleaned and aggregated data by connecting to Azure SQL Database or directly from Azure Blob Storage.

### Dataset Location

- **Raw Data**: The datasets are stored in **Azure Blob Storage** under a container called `olympics-data-2024`.
- **Processed Data**: After processing and analysis, the aggregated data is stored in **Azure SQL Database** or exported back to Azure Blob Storage.

## How to Run the Project

### 1. **Set up Azure Blob Storage (ABS)**:
   - Upload the datasets to Azure Blob Storage using Azure Portal or Azure CLI.
   
### 2. **Set up Azure Data Factory (ADF)**:
   - Create a Data Factory instance in the Azure portal.
   - Define pipelines in ADF to automate the ingestion and transformation of data from Blob Storage to SQL Database.
   - Set up scheduled triggers to automate the data pipeline and processing.

### 3. **Run Analysis Using Python**:
   - Load the datasets into Python and perform data transformations and analysis.

### 4. **Export Results**:
   - Export the results of the analysis back to Azure Blob Storage or Power BI for reporting.
