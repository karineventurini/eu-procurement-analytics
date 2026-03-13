# EU Public Procurement Analytics (2018–2023)

## Overview

This project analyzes European public procurement contract award data from 2018 to 2023, using official TED (Tenders Electronic Daily) datasets. The objective is to explore procurement trends, supplier activity, contract volume, and economic value through a structured data pipeline and interactive Power BI dashboard.

The project demonstrates end-to-end data analytics workflow including data inspection, cleaning, modeling, and visualization.

---

## Objectives

The analysis focuses on answering key business questions:

- How has the number of awarded contracts evolved over time?
- What is the year-over-year growth of contract volume?
- Who are the most active suppliers?
- What is the total and median economic value of contracts?
- How is contract value distributed across suppliers and time?

---

## Dataset

Source:  
TED – Tenders Electronic Daily (European Union public procurement data)

Coverage:

- Years: 2018–2023
- Scope: EU public contract awards
- Records: >1.6 million contract awards

Key fields:

- contract_id
- supplier_name
- supplier_id
- award_date
- award_value_euro
- number_offers

---

## Data Pipeline

The project follows a structured ETL approach:


Dimensional model:

- fact_contract_awards_clean → contract-level data
- fact_contract_value → contract economic value
- dim_supplier → supplier dimension
- dim_date → calendar dimension

---

## Tools Used

- Python (Pandas) – data cleaning and preparation
- Power BI – data modeling and dashboard visualization
- GitHub – version control and project documentation

---

## Dashboard

The Power BI dashboard contains two analytical pages:

### Contract Volume & Trends

Key metrics:

- Total Contracts
- Year-over-Year Growth
- Average Offers per Contract
- Unique Suppliers

Visualizations:

- Monthly contract trend
- Top suppliers by number of contracts
- Current vs previous year comparison

Screenshot:

![Contract Volume & Trends](docs/dashboard_volume_trends.png)

---

### Economic Analysis

Key metrics:

- Total Contract Value (€)
- Median Contract Value (€)

Visualizations:

- Total contract value by year
- Monthly contract value trend
- Top suppliers by contract value

Screenshot:

![Economic Analysis](docs/dashboard_economic_analysis.png)

---

## Key Insights

Key findings include:

- Steady increase in procurement activity between 2018 and 2022
- Significant variation in contract values, with highly skewed distribution
- Concentration of contract value among a subset of suppliers
- Strong temporal trends visible at yearly and monthly levels

---

## Repository Structure

```
eu-procurement-analytics/
│
├── data/
│   ├── raw/
│   ├── staging/
│   ├── processed/
│   └── mart/
│
├── notebook/
│   └── 01_staging_inspection.ipynb
│
├── powerbi/
│   └── eu-procurement-analytics-dashboard.pbix
│
├── docs/
│   ├── dashboard_volume_trends.png
│   └── dashboard_economic_analysis.png
│
└── README.md
```

---

## Skills Demonstrated

- Data cleaning and validation
- Dimensional data modeling
- ETL pipeline design
- Data visualization and dashboard development
- Analytical interpretation of procurement data

---

## Author

Karine G. Venturini de Oliveira  
Junior Data Analyst  
```

---

 
