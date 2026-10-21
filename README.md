[Click here to download the interactive .pbix file from Google Drive](https://drive.google.com/file/d/1fhK1BRF3ln2qX40kn_GkBxwAK_lOgQ_1/view?usp=sharing)

# LA-Crime-Power-BI-analytics-
End-to-end Power BI data analytics project modeling 1M+ LA crime records into a 6-dimension Star Schema.

# Los Angeles Municipal Crime Analytics (Power BI)

## 📌 Project Overview
This project performs an end-to-end business intelligence analysis on raw municipal crime data from Los Angeles (1M+ records). The goal was to transform an un-normalized flat file into a performant, relational **Star Schema** in Power BI to answer key operational and demographic questions regarding crime trends, geographic concentrations, and victim vulnerability profiles.

---

## 🏗️ Data Architecture & Star Schema
The dataset was cleaned and structured using **Power Query** into 1 central Fact table and 6 Dimension tables, establishing active `1-to-many` single-direction relationships:

* **Fact Table:** `Fact_Crime` 
* **Dimension Tables:**
  * `Dim_Area`: Geographic patrol area names
  * `Dim_Crm_Cd`: Crime classification descriptions 
  * `Dim_Premis`: Premise descriptions 
  * `Dim_Weapon`: Weapon category descriptions 
  * `Dim_Status`: Case status descriptions 
  * `DateTable`: Continuous date hierarchy (Date, Year, Quarter, Month, DayOfWeek)


---

## 🛠️ Data Cleaning & ETL Process (Power Query)
* **Data Sanitization:** Handled null/missing values across weapon descriptions and victim attributes.
* **Column Optimization:** Removed redundant text fields from the Fact table to optimize engine performance and storage footprint.

---

## 📊 Business Questions Answered

### 1. Crime Trends Over Time
Analyzed temporal shifts across years, quarters, and days of the week to identify peak operational risk hours for law enforcement resource deployment.

### 2. Geographic & Divisional Distribution
Identified high-volume patrol areas and premise concentrations to highlight specific locations experiencing disproportionate crime rates.

### 3. Victim Demographic Profiles
Examined vulnerability matrices crossing victim age groups and sex against specific crime types.

---

## 🖥️ Dashboard Previews

### Operational Crime Overview


### Victim Demographic Vulnerability Analysis


---

## 🔧 Tools & Technologies
* **Power BI Desktop:** Star Schema Data Modeling, DAX Measures, Interactive Visualizations
* **Power Query:** ETL, Data Cleaning, Normalization, Data Type Mapping
