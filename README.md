# Cholera-Capstone-Project

Predictive Analytics for Cholera Outbreaks (2000–2023)

This project applies data science and machine learning to predict cholera outbreak severity based on historical surveillance data, enabling proactive public health responses. The analysis supports goals of the WHO and GTFCC to reduce cholera deaths through early intervention, better targeting, and resource optimization.

1. # Project Overview

   Project_Capstone dane By: Huruma Innocent, ID:25514
   Course: Introduction to Big Data Analytics  
   Institution Adventist University of Central Africa (AUCA)  
   Year: 2024–2025  
   Sector: Health  
   Dataset Source: [WHO Cholera Cases and Deaths](https://www.who.int/emergencies/surveillance/cholera-cases-and-deaths)  
   Tools: Python, Scikit-learn, Pandas, GeoPandas, Power BI

2. Problem Statement
   Cholera remains a global public health threat, causing thousands of deaths annually, especially in low- and middle-income countries. Traditional reactive responses delay intervention, increasing mortality and spread.

**Predict annual cholera case trends and outbreak severity using historical, environmental, and regional health data.**

## Methodology

### 🔹 Step 1: Data Collection & Cleaning

- Source: WHO (2000–2023), 1,094 country-year records
- Recalculated Case Fatality Rate (CFR)
- Removed outliers (CFR > 50%)
- Created categorical variable `Outbreak_Size`
- Encoded regions and normalized features
  ![alt text](<Data Befor clean.jpg>) ![alt text](<Clean Dataset.jpg>) ![alt text](<Data After Clean.jpg>)

### 🔹 Step 2: Exploratory Data Analysis (EDA)

- Global trends of cholera cases and deaths
  ![alt text](image-2.png)
- CFR comparison by WHO region
- Top 10 countries by total cases
  ![alt text](image-1.png)
- Correlation heatmaps of CFR, Incidence Rate, and Total Cases
  ![alt text](Map.jpg)

### 🔹 Step 3: Machine Learning

- **Model**: Random Forest Classifier
  ![alt text](<Machine Learning Model.jpg>)
- **Target**: `Outbreak_Size` (Small, Medium, Large, Epidemic)
- **Features**: Year, CFR, Incidence per million, Region (encoded)
- **Evaluation**: Confusion matrix, classification report
  ![alt text](Report-1.jpg)

### 🔹 Step 4: Innovation

- `risk_alert()` function: Flags countries with high CFR and case volume
- Geo-mapping of cholera hotspots using GeoPandas + Contextil

3. Power BI Dashboard

An interactive dashboard was developed in **Power BI** to visualize:

- Global case trends (2000–2023)
  ![alt text](<Global Cholera Trends Over Time.jpg>)
- Region-wise fatality and outbreak size
  ![alt text](<Cases by Subregion.jpg>)
- Top 10 affected countries
  ![alt text](<Top 10 Countries by Cases-1.jpg>)
- Map visual with slicers for year and region
  ![alt text](Map-1.jpg)
  Dashbord
  ![alt text](Dashbord.jpg)

Let it serve as a reminder that excellence, integrity, and commitment matter  
whether in data science, public health, or everyday life.
