# 🚗 NYC Collision Data Analysis & Dashboards

**Author:** Aman — Data Analyst  
**Repository:** NYC_Collision_Data_Analysis  
**Date:** 2025

---

## 📌 Overview

This project transforms raw New York City vehicle collision records into a concise, actionable analytics deliverable: interactive Excel dashboards and accompanying visual assets. The work prioritizes high-impact insights, reproducibility, and stakeholder usability — designed to inform operations, policy, and resource allocation decisions.

---

## Key Deliverables

- `Collision DashBoards.xlsm`  
  Excel dashboard workbook containing pivot-driven reports, slicers, and macro-enabled controls to support deep interactive exploration.

- `NYC_Collisions.csv`  
  Cleaned and preprocessed collision dataset used as the single source of truth for the dashboards.

- `NYC_Collisions_data_dictionary.csv`  
  Field definitions, types, and provenance notes that enable reproducibility and governance.

- Visual assets:  
  - `Dashboard 1.png`, `Dashboard 2.png` — high-fidelity screenshots of the dashboard layout and key views.  
  - `Ob 1.PNG`, `Ob2.PNG`, `Ob3.PNG` — component-level visualizations highlighting important patterns.  
  - `Color.xlsx` — color palette and style guide for consistent branding across reports.  
  - `Taskes.PNG` — analytical roadmap and task breakdown.

---

## 🗂 Dataset
The analysis is based on:  
- **NYC_Collisions.csv** → Contains detailed collision records.  
- **NYC_Collisions_data_dictionary.csv** → Explains each field in the dataset.  

### Key Information Included:
- **Collision ID** – Unique identifier for each record  
- **Date & Time** – Timestamp of the collision  
- **Location** – Borough, street names, latitude & longitude  
- **Contributing Factor** – Primary reason behind the collision  
- **Vehicle & Person Info** – Vehicle types, and counts of persons, pedestrians, cyclists, and motorists injured or killed

---

## 🛠 Tools Used
- Excel

---

## 🎯 Objectives

- Surface temporal and spatial patterns in collision incidence (by borough, time-of-day, day-of-week).  
- Identify high-risk locations and demographic cost drivers.  
- Provide stakeholders with a tool to filter, interrogate, and export curated views for decision-making.  
- Maintain a clean, documented dataset and a clear data dictionary to support audits and enhancements.

---

## How to Use

### Requirements
- Microsoft Excel with macro support (for `.xlsm` functionality).
- Basic familiarity with PivotTables, slicers, and Excel macros.

### Quick Start
1. Clone or download this repository.  
2. Place `NYC_Collisions.csv` in the same folder as `Collision DashBoards.xlsm` (or update the workbook data connection).  
3. Open `Collision DashBoards.xlsm` in Excel and *Enable Macros* (trusted location recommended).  
4. Use slicers to filter by borough, date-range, time-of-day, and contributing factors.  
5. Export charts or snapshots as needed for presentations or reports.

---

## 🔍 Key Findings & Observations
### 📌 Observation 1  
The majority of accidents involved **passenger vehicles**, with many caused by **driver inattention and distraction**.  

### 📌 Observation 2  
**Tuesdays and Fridays** recorded the highest accidents, with peaks during **evening commute hours**.  

### 📌 Observation 3  
Injuries peaked during specific months and hours, highlighting a need for targeted **safety measures**.  

---

## 📊 Interactive Dashboards
Two **Power BI Dashboards** were developed to visualize and explore the data.  

### 🔹 Dashboard 1 – *Trends & Factors*  
- High-level overview of collisions  
- Trends over time  
- Top contributing factors  

![Dashboard 1](Dashboard%201.png)

### 🔹 Dashboard 2 – *Geographic Analysis*  
- Map view of accident hotspots  
- Breakdown by borough and street-level insights  

![Dashboard 2](Dashboard%202.png)

---

## Analytical Methodology (summary)

1. **Data ingestion & cleaning** – filter duplicates, normalize datetime fields, standardize categorical variables (e.g., contributing factors, vehicle type), validate geographic fields (borough, intersection).  
2. **Feature engineering** – derive `time_of_day`, `day_of_week`, severity flags, and aggregated metrics (counts, injury counts, fatality counts).  
3. **Validation & governance** – reconcile counts with source, document field transformations in the data dictionary.  
4. **Visualization & UX** – design dashboards prioritizing clarity: concise KPIs, temporal trend charts, borough comparisons, and hotspot visualizations.  
5. **Delivery** – packaged as macro-enabled workbook with visual assets for immediate stakeholder consumption.

---

## Recommended Next Steps / Extensions

- **Geospatial mapping:** integrate with a mapping engine (Power BI, Tableau, or Folium/Kepler) to produce interactive hotspot layers.  
- **Predictive modeling:** time-series forecasting and classification to predict high-risk windows or intersections.  
- **Automated ETL:** scheduled pipeline to pull the latest NYC Open Data CSV and refresh dashboard datasets.  
- **Cross-dataset augmentation:** enrich collision records with weather, traffic volume, and socioeconomic indicators to uncover root causes.

---

## Best Practices & Notes

- Treat `NYC_Collisions.csv` as the canonical source; any enrichment should be documented and versioned.  
- Use the `NYC_Collisions_data_dictionary.csv` for field-level explanations and to onboard stakeholders quickly.  
- Store macro-enabled workbooks in trusted locations to avoid Excel macro security prompts during demos.

---

## 📬Contribution and Contact
For questions or feedback, feel free to connect:  
📧 Email → theanalyst.aman@gmail.com  
🔗 LinkedIn → www.linkedin.com/in/aman-singh-negi-482197310
---
