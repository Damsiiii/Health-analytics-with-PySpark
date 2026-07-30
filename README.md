# Student Health Analytics using PySpark

A Big Data analytics project that leverages **Apache Spark (PySpark)** to clean, transform, analyze, and visualize student health data. The project demonstrates scalable data preprocessing, feature engineering, statistical analysis, and MongoDB integration using a healthcare-inspired dataset.

---

## Project Overview

This project builds an end-to-end health analytics pipeline capable of processing student biodata to identify health risks and generate actionable insights.

The workflow includes:

- Data ingestion using Apache Spark
- Data cleaning and preprocessing
- Missing value imputation
- Feature engineering
- Health risk analysis
- Aggregations and reporting
- MongoDB integration

The objective is to demonstrate practical data engineering and analytics techniques on structured healthcare data.

---

## Technologies Used

- Python
- Apache Spark (PySpark)
- Google Colab
- Pandas
- Matplotlib
- MongoDB
- PyMongo

---

## Dataset

Student Health Dataset

**100 student records**

Features include:

- Student Information
- Height
- Weight
- Blood Group
- Department
- Academic Year
- Blood Pressure
- Cholesterol Level

---

# Project Architecture

```
CSV Dataset
      │
      ▼
Data Loading
      │
      ▼
Data Cleaning
      │
      ▼
Missing Value Imputation
      │
      ▼
Feature Engineering
      │
      ▼
Health Risk Analysis
      │
      ▼
MongoDB Storage
      │
      ▼
Reporting & Visualization
```

---

# Features

## Data Loading

- Loaded CSV dataset using Apache Spark
- Inferred schema automatically
- Verified dataset dimensions and data types

---

## Data Cleaning

Implemented several preprocessing techniques:

- Detected invalid medical values
- Replaced zero values with NULL
- Identified missing values
- Preserved all records during cleaning

---

## Missing Value Imputation

Used domain-aware imputation instead of deleting records.

Applied:

- Gender-wise mean for Height
- Gender-wise mean for Weight
- Department-wise mean for Cholesterol

This maintained dataset integrity while minimizing statistical bias.

---

## Feature Engineering

Generated several analytical features including:

- Body Mass Index (BMI)
- BMI Category
- High Blood Pressure Flag
- At-Risk Classification
- Risk Explanation

---

## Health Risk Analysis

Students were classified as at-risk based on:

- Obesity or Overweight BMI
- High Blood Pressure
- High Cholesterol

Each record includes a detailed explanation describing the detected risk factors.

---

## Data Analysis

Generated analytical insights including:

- Average BMI by Department
- Department-wise At-Risk Percentage
- Mean Blood Pressure by Academic Year
- BMI Pivot Tables
- Highest-Risk Student Ranking

---

## Data Visualization

Created visualizations for:

- BMI Category Distribution
- Health Risk Trends

---

## MongoDB Integration

Implemented MongoDB connectivity using PyMongo.

Features include:

- Database connection
- Spark DataFrame to JSON conversion
- Bulk document insertion
- Retrieval and verification of stored records

---

# Project Structure

```
project/
│
├── dataset/
├── notebooks/
├── cleaned_data/
├── visualizations/
├── mongodb/
└── README.md
```

---

# Key Skills Demonstrated

- Big Data Processing
- Apache Spark
- Data Cleaning
- Missing Value Imputation
- Feature Engineering
- Healthcare Data Analytics
- Data Visualization
- MongoDB Integration
- ETL Pipeline Development
- Statistical Analysis

---

# Results

The project successfully:

- Processed student health records using PySpark
- Cleaned and standardized medical data
- Engineered health-related features
- Identified at-risk individuals
- Generated department-level health insights
- Stored processed data in MongoDB for future querying

---

# Learning Outcomes

This project strengthened my understanding of:

- Distributed data processing with Apache Spark
- Real-world data preprocessing techniques
- Feature engineering for healthcare datasets
- Analytical reporting using PySpark
- NoSQL database integration
- End-to-end ETL pipeline development

---

# Future Improvements

- Deploy the pipeline on AWS EMR
- Automate workflows using Apache Airflow
- Containerize with Docker
- Integrate Apache Kafka for streaming data
- Develop an interactive Power BI dashboard
- Implement machine learning models for health risk prediction

---
