 # EU Public Procurement Analytics (2018–2023)

## Overview

This project analyzes European public procurement contract award data from 2018 to 2023 using official TED (Tenders Electronic Daily) datasets.

The objective is to explore procurement trends, supplier activity, contract volume, and economic value through a structured data analysis workflow and an interactive Power BI dashboard.

The project demonstrates an end-to-end data analytics workflow including data inspection, cleaning, modeling, and visualization.

---

## Objectives

The analysis focuses on answering key business questions:

- How has the number of awarded contracts evolved over time?
- What is the year-over-year growth of contract volume?
- Who are the most active suppliers?
- What is the total and median economic value of contracts?
- How is contract value distributed across suppliers and over time?

---

## Dataset

**Source**

TED – Tenders Electronic Daily  
Official European Union public procurement data.

**Coverage**

- Years: 2018–2023  
- Scope: EU public contract awards  
- Records: >1.6 million contract awards  

**Key fields**

- `contract_id`
- `supplier_name`
- `supplier_id`
- `award_date`
- `award_value_euro`
- `number_offers`

---

## Data Pipeline

The project follows a structured data preparation pipeline:

1. **Data inspection**  
   Initial exploration of TED contract award datasets.

2. **Data cleaning**  
   - handling missing values  
   - standardizing supplier information  
   - validating contract records

3. **Data transformation**  
   Creation of structured analytical tables for reporting and dashboard development.

4. **Dimensional modeling**

The analytical dataset includes:

- **fact_contract_awards_clean** → contract-level information  
- **fact_contract_value** → economic value of contracts  
- **dim_supplier** → supplier dimension  
- **dim_date** → calendar dimension

---

## Tools Used

- **Python (Pandas)** – data cleaning and preparation  
- **Power BI** – data modeling and dashboard visualization  
- **GitHub** – version control and project documentation  

---

## Dashboard

The Power BI dashboard contains two analytical pages.

---

### Contract Volume & Trends
 
**Key metrics**

- Total Contracts
- Year-over-Year Growth
- Average Offers per Contract
- Unique Suppliers

**Visualizations**

- Monthly contract trend
- Top suppliers by number of contracts
- Current vs previous year comparison

![Contract Volume & Trends](./Immagini/contract_volume_trends.png)

  ---

### Economic Analysis
 
**Key metrics**

- Total Contract Value (€)
- Median Contract Value (€)

**Visualizations**

- Total contract value by year
- Monthly contract value trend
- Top suppliers by contract value
 
![Economic Analysis](./Immagini/contract_value_analysis.png)

## Key Insights

Main findings from the analysis include:

- A steady increase in procurement activity between 2018 and 2022
- Large variability in contract values, indicating a highly skewed distribution
- Concentration of economic value among a subset of suppliers
- Clear temporal trends visible at both yearly and monthly levels

---

## Repository Structure

eu-procurement-analytics/
│
├── data/
│ └── mart/
│ ├── dim_date.csv
│ └── dim_supplier.csv
│
├── docs/
│ └── progetto2_Capstone_Epicode.docx
│
├── images/
│ ├── Assegnato valore contrattuale Analysis.png
│ └── Volume contrattuale & Trends.png
│
├── notebooks/
│ ├── 01_staging_inspection.ipynb
│ └── 02_ted_data_cleaning.ipynb
│
└── README.md


---

## Skills Demonstrated

- Data cleaning and validation
- Exploratory data analysis
- Dimensional data modeling
- ETL pipeline design
- Data visualization and dashboard development
- Analytical interpretation of large-scale procurement data

---

## Author

Karine G. Venturini de Oliveira  
Junior Data Analyst

 














