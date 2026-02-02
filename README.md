# Aadhaar Analytics Framework: System Stress, Inclusion & Demand Intelligence

## Overview
This project develops a comprehensive analytical framework to extract policy-relevant insights from Aadhaar enrolment and update data published by UIDAI. By transforming routine administrative records into interpretable indices and visualisations, the project enables monitoring of system stress, mobility-driven demand, inclusion gaps, lifecycle coverage, and future service pressure.

The framework is built exclusively using the Aadhaar datasets provided for the challenge and is designed to support data-driven governance, proactive planning, and targeted operational interventions.

---

## Project Components

The project consists of five integrated analytical modules:

### 1. Aadhaar Stress Index (ASI)
Measures operational pressure on Aadhaar infrastructure by combining update load, age-driven demand, transaction volatility, and update intensity. ASI acts as an early-warning indicator for system stress at national, state, and district levels.

### 2. Aadhaar Mobility Pulse (AMP)
Captures short-term population movement using adult Aadhaar enrolment and update patterns. AMP helps identify regions experiencing migration-driven demand surges.

### 3. Aadhaar Inclusion Deficit Index (AIDI)
Identifies regions with persistently low Aadhaar activity, indicating potential gaps in access, awareness, or service reach.

### 4. Aadhaar Lifecycle Coverage Score (ALCS)
Evaluates whether Aadhaar enrolment and update services are balanced across lifecycle stages—early childhood, school age, and adulthood.

### 5. Aadhaar Demand Forecast Score (ADFS)
Provides a forward-looking estimate of near-term Aadhaar service demand based on recent activity trends.

---

## Datasets Used

All analyses use UIDAI-provided datasets:
- Aadhaar Enrolment Data
- Aadhaar Biometric Update Data
- Aadhaar Demographic Update Data

### Key Columns
- Date  
- State  
- District  
- Pincode  
- Age-group-wise enrolment and update counts  

No external datasets were used.

---

## Data Cleaning & Preprocessing

- Standardised date formats and geographic fields  
- Aligned schema and age-group columns across datasets  
- Merged datasets using date, state, district, and pincode  
- Created derived metrics such as total enrolments, updates, and transactions  
- Retained missing dates and administrative inconsistencies to preserve raw signal integrity  

A conservative cleaning approach was adopted to avoid artificial smoothing or imputation.

---

## Methodology Summary

- Construction of transparent, explainable indices using normalized components  
- Temporal analysis at daily and monthly levels  
- Geographic aggregation at national, state, and district scales  
- Visual analysis using bar charts, line plots, heatmaps, and geospatial maps  

All index formulas and weights are explicitly documented in the notebooks.

---

## Visualisations

The project includes:
- State-wise and district-wise ASI bar charts  
- Monthly trend analysis  
- District heatmaps for stress persistence  
- National and sub-national choropleth maps  
- Lifecycle activity distribution plots  

Each visualisation is accompanied by result-driven interpretations.

---

## Repository Structure

.
├── Data_cleaning.ipynb
├── ASI.ipynb
├── AMP.ipynb
├── AIDI.ipynb
├── ALCS.ipynb
├── ADFS.ipynb
├── README.md


---

## Key Outcomes

- Converts Aadhaar administrative data into actionable governance intelligence  
- Enables early detection of system stress and demand surges  
- Highlights inclusion gaps and lifecycle imbalances  
- Supports district-level, evidence-based decision-making  

---

## Tools & Libraries

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- GeoPandas  

---

## Disclaimer

This project is an analytical exercise conducted using UIDAI-provided datasets for a government challenge. All insights reflect patterns in reported administrative data and do not represent official UIDAI assessments or policy positions.
