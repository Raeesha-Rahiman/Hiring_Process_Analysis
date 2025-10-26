# Hiring_Process_Analysis

## Overview 
This project analyzes the **hiring timeline across various job vacancies**, focusing on how much time it takes for a position to move from the **application stage** to the **filled stage**.

The goal is to identify **bottlenecks and delays** in the recruitment process, improve **time-to-hire efficiency**, and provide **data-driven insights** to optimize overall hiring performance.

The analysis is performed using:
- **Excel** for initial data cleaning and exploration  
- **SQL** for data extraction and transformation  
- **Python** for data analysis and hypothesis testing  
- **Power BI / Dashboard** for visualization and reporting

- 
## 🎯 Objectives
- **Identify the stages with the highest delays and vacancy drop-offs (bottlenecks)** in the hiring funnel.  
- **Compare BU (Business Unit) regions** to determine which areas have the **highest and lowest vacancy fill rates**.  
- **Compare part-time and full-time vacancies** to assess differences in hiring efficiency.  
- **Analyze monthly trends** to identify **peak and low hiring conversion periods**.  
- **Detect off-season hiring months** to support better **resource planning and forecasting**.



- 🗂️ Dataset Description

This project uses a single dataset that tracks the hiring process for different vacancies across various Business Units (BU Regions).
Each record represents one vacancy and the timeline of its recruitment stages.

| Column Name         | Description                                                   |
| ------------------- | ------------------------------------------------------------- |
| **ID**              | Unique identifier for each vacancy.                           |
| **FP**              | Represents the financial period or month of hiring.           |
| **BU Region**       | Business Unit region responsible for the vacancy.             |
| **Approved**        | Date when the vacancy was approved.                           |
| **On hold**         | Date when the vacancy was temporarily paused (if applicable). |
| **Sourcing start**  | Date when candidate sourcing began.                           |
| **Interview start** | Date when interviews started.                                 |
| **Interview end**   | Date when interviews concluded.                               |
| **Offered**         | Date when the offer was made to the candidate.                |
| **Filled**          | Date when the vacancy was filled (hired).                     |
| **Status**          | Current status of the vacancy (e.g., Filled, On hold, Open).  |



🔄 Workflow Description
| Step | Stage                           | Tool                                     | Description                                                                                                                                                                             |
| ---- | ------------------------------- | ---------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1    | **Data Cleaning & Preparation** | **Excel**                                | Cleaned 12 monthly vacancy files and **combined them into a single master dataset**. Removed duplicates, standardized column names, corrected date formats, and handled missing values. |
| 2    | **Data Ingestion**              | **SQL**                                  | Loaded the cleaned and consolidated Excel dataset into SQL tables for structured querying.                                                                                              |
| 3    | **Data Transformation (ETL)**   | **SQL**                                  | Performed data transformation — calculated time durations between recruitment stages, filtered completed records, and created status-based summaries.                                   |
| 4    | **Data Analysis**               | **Python (Pandas, Matplotlib, Seaborn)** | Conducted exploratory data analysis (EDA), visualized hiring patterns, and identified stage-wise delays.                                                                                |                                                                                     |
| 6    | **Visualization**               | **Power BI**                             | Built an interactive dashboard highlighting BU region performance, monthly hiring trends, and stage-wise process timelines.                                                             |
| 7    | **Reporting**                   | **Markdown / GitHub**                    | Documented the workflow, results, and key business insights in this README report.


## 📊 Key Insights
### ⏳ Process Efficiency
The average time-to-fill varies significantly across BU Regions.
Certain stages like Interview Start → Offered and Offered → Filled have the longest delays, indicating approval or negotiation slowdowns.

### 🌍 Regional Comparison
Some BU Regions maintain a faster average hiring cycle than others.
Low-performing regions show higher on-hold rates and longer sourcing periods.

### 🧩 Part-Time vs Full-Time
Full-time roles generally take longer to fill compared to part-time roles due to extended interview and negotiation processes.

### 📅 Monthly Trends
Off-season months can be used for planning and training HR staff

## Dashboard

<img width="962" height="535" alt="image" src="https://github.com/user-attachments/assets/e2573e15-5c42-4249-8cf0-689fd3127a54" />


👩‍💻 Author

Raeesha Rahiman
Aspiring Data Analyst | Skilled in SQL, Python, Excel, and Power BI
📍 Abu Dhabi















