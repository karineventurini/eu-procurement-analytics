 # EU Procurement Analytics (2018–2023)

## Project Overview
This project analyzes European public procurement contract awards published on the EU Tenders Electronic Daily (TED) platform between 2018 and 2023.
The objective is to provide a structured analytical view of procurement activity, supplier concentration, and competitive dynamics using a professional data analytics workflow.

## Business Questions
- How many public procurement contracts were awarded across the EU between 2018 and 2023?
- How many unique suppliers participated in awarded contracts during the period?
- How concentrated is contract allocation among top suppliers?
- How does procurement activity evolve over time across EU countries?
- How competitive are public tenders in terms of the average number of offers received?

## Data Sources
- European Union – Tenders Electronic Daily (TED)
- Contract Award Notices (CAN)
- Period: 2018–2023

## Data Processing & Modeling
The raw procurement data were ingested and inspected to ensure consistency and completeness before analysis.
A structured data model was then designed using a star schema approach, with a contract-level fact table and dedicated dimensions for suppliers and dates.
Data cleaning, type normalization, and null handling were performed in Python to produce an analytics-ready dataset suitable for KPI computation and business intelligence reporting.

## Analytical Tools
- Python (Pandas) for data cleaning, transformation, and modeling
- Power BI for dimensional modeling, DAX measures, and interactive reporting

## Key Metrics
- Total number of awarded contracts
- Total number of unique suppliers
- Average number of offers per contract
- Contract awards trend by year
- Top suppliers by number of awarded contracts

## Key Insights
- Public procurement activity shows a sustained increase over the analyzed period, with a noticeable acceleration after 2019.
- A relatively small number of suppliers account for a significant share of awarded contracts, indicating a measurable level of supplier concentration.
- Competition levels, measured by the average number of offers per contract, vary considerably across years and procurement categories.

## Deliverables
- Interactive Power BI dashboard for exploratory and executive-level analysis
- Clean, analytics-ready dataset structured for KPI computation
- Reproducible data analytics workflow documented in the repository

## Methodological Notes
The analysis is based exclusively on awarded contract data published through the TED platform and does not include tender notices that did not result in an award.
All metrics are computed using cleaned and standardized data to ensure comparability across time and entities.
The project prioritizes transparency and reproducibility, with clear separation between raw data, transformed datasets, and analytical outputs.
