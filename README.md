### Spotify-Data-Pipeline-ETL-AWS
This project builds an automated data pipeline for extracting, transforming, and analyzing Spotify data using AWS services. AWS Lambda fetches data from the Spotify API, processes it, and stores it in Amazon S3. AWS Glue and Amazon Athena enable structured querying and efficient analytics.

### Overview
This project builds a data pipeline to collect, process, and analyze Spotify data using AWS services. It fetches data from the Spotify API, processes it with AWS Lambda, and stores it in Amazon S3 in an organized way. AWS Lambda automatically extracts data at scheduled times using Amazon CloudWatch. The data is cleaned, formatted, and stored in S3 for further analysis. AWS Glue and Amazon Athena help structure and query the data to gain useful insights. This pipeline is scalable, automated, and makes Spotify data analysis easier and more efficient.

### Architecture Diagram
![image](https://github.com/user-attachments/assets/0277a17d-2160-4c09-8630-12883838ca6f)

## Methodology

### 1. Data Extraction  
**Goal:** Get data from Spotify API and store it in Amazon S3.  

**How it works:**  
- AWS Lambda fetches Spotify data and saves it in S3.  
- Amazon CloudWatch triggers Lambda daily to automate the process.  

### 2. Data Transformation  
**Goal:** Clean and prepare the data for analysis.  

**How it works:**  
- AWS Lambda reads the raw data from S3.  
- It cleans, organizes, and filters the data.  
- The processed data is saved in another S3 bucket.  

### 3. Data Loading & Analysis  
**Goal:** Organize data for easy querying and analysis.  

**How it works:**  
- AWS Glue Crawler scans the data and creates a structured catalog.  
- AWS Glue Data Catalog organizes the data for better access.  
- Amazon Athena allows users to run SQL queries for insights.  

## Key Observations  
- Successfully fetched Spotify data and stored it in Amazon S3.  
- Processed and structured data for better querying.  
- Enabled SQL-based analysis using Amazon Athena.  

## Significance  
- Provides a scalable and automated way to process Spotify data.  
- Helps in generating insights for recommendations, trends, and music popularity analysis.  


