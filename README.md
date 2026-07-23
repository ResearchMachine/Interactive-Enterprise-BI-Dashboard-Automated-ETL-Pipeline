# Interactive Enterprise BI Marketing Funnel & ETL Pipeline

A production-ready Full-Stack Data Product built with **Streamlit** and **Plotly Express** designed to automate cross-channel marketing campaign auditing, data extraction, and econometric KPI validation.

## 🎯 The Problem & The Solution

In large enterprises, marketing research and media agency reports often arrive scattered across hundreds of multi-sheet Excel files with mismatched schemas, shifting tables, and messy naming conventions. 

This repository provides a scalable **Data Ingestion Layer (ETL)** coupled with a clean interactive web application that transforms fragmented data into instantly scannable, data-driven business insights.

## 🛠️ Core Capabilities

* **Resilient Data Ingestion**: Features an advanced cleaning layer that handles missing data (`.notna()`), strips formatting anomalies, drops programmatic artifacts (e.g., `Total*`), and maps raw multi-lingual strings to unified relational schema names.
* **Strict Schema Type Validation**: Safely converts unstructured text payloads to programmatically sound metrics via explicit `pd.to_numeric(errors="coerce")` type casting.
* **Multi-Touch Funnel Optimization**: Aggregates raw contact capacity (OTS), reach metrics, and performance analytics into an interactive visual conversion funnel across three unique business channels: Core Business (**АКБ**), Online, and Mobile App (**App**).
* **Advanced Multi-KPI Simulators**: Interactive tabs mapping CPRP vs. Reach Capacity share and Bubble chart dimensions mapping Econometric Coefficients vs. Volumetric Contribution vs. Media Budget Allocation.

## 💻 Tech Stack

* **Framework**: Streamlit (Web App Interface)
* **Data Engineering**: Python 3, Pandas, OpenPyXL, Base64 Stream Handling
* **Data Visualization**: Plotly Express (Funnel, Scatter, Histograms, Grouped Bars)

## 📦 How to Run

1. Clone the repository and install the requirements:
   ```bash
   pip install streamlit pandas plotly openpyxl
   ```
2. Launch the Streamlit application:
   ```bash
   streamlit run app.py
   ```
3. Choose the build-in Base64 encoded Demo Dataset or upload your own enterprise `.xlsx` marketing report to test the live parser!
