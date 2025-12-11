# RealEstate-NYC-Planning-Analytics
Interactive Power BI analytics on 500+ NYC Planning projects (ZAP): trends by borough, status, admins, and time.
# Urban real estate development analytics — NYC Planning (ZAP)

Interactive analytics on 500+ NYC Planning projects across boroughs and statuses, built with Python (pandas) for preprocessing and Power BI for visualization. This end-to-end case study reveals trends in development activity, pipeline maturity, seasonal patterns, and administrator workloads.

## 🚀 Highlights
- End-to-end pipeline: sourcing → cleaning → modeling → interactive dashboard
- Key insights:
  - Manhattan, Brooklyn, Queens account for ~72% of projects
  - ~86% of the pipeline is completed (mature activity)
  - Seasonal spike in Q4 (Oct–Nov)
  - A handful of admins manage a high share of projects
- Tools: Python (pandas), Excel, Power BI, DAX

## 📂 Project structure
- `/data` — sample_cleaned.csv (trimmed), data dictionary
- `/notebooks` — cleaning_pipeline.ipynb (ETL/preprocessing)
- `/dashboard` — Power BI file (pbix) and screenshots
- `/docs` — case study, architecture diagram
- `/scripts` — optional ETL scripts

## 📊 Dashboard overview
- Summary cards: total projects, admins, applicants, boroughs
- Visuals:
  - Projects by borough (bar)
  - Status distribution (pie)
  - Projects by year (bar)
  - Monthly trend (line)
  - Top 10 admins (table)
  - Geospatial map (Power BI Map)
- Filters: time range, borough, status

## 🧪 Data
- Source: NYC Zoning Application Portal (ZAP)
- Granularity: project-level records
- Columns: Project_id, Applicant_Name, Project_Name, Status, Borough, City, LastUpdated, Application_Administrator, Month
- Note: This repo includes a trimmed sample dataset for demonstration.

## 🛠️ Repro steps
1. Clone the repo
2. Open `/notebooks/cleaning_pipeline.ipynb` and run preprocessing
3. Load `sample_cleaned.csv` into Power BI
4. Open `/dashboard/Real_estate_RaviTeja_Akash.pbix` (or recreate visuals following docs/CaseStudy.md)
5. Use filters to explore trends

## 🧭 Architecture
End-to-end flow:
City Planning (ZAP) → Extraction (Manual/API) → Cleaning (Excel/Python) → Aggregation → Storage (CSV/PBI dataset) → Visualization (Power BI)

![Architecture Diagram](docs/architecture.png)

## 📸 Screenshots
!Summary & Boroughs<img width="423" height="313" alt="Boroughs" src="https://github.com/user-attachments/assets/19fe34b5-1ee8-45e2-a3ca-7cd756111d07" />

!Status & Year <img width="417" height="307" alt="status " src="https://github.com/user-attachments/assets/a7d0490d-d09c-4eef-852e-420f2f0b6325" />

!Monthly Trend<img width="587" height="332" alt="trend" src="https://github.com/user-attachments/assets/34f23b6c-7f48-449b-9331-cc719d890ce7" />

!Top Admins <img width="261" height="329" alt="top10 " src="https://github.com/user-attachments/assets/a2aaea70-870d-43c3-96d5-ed6d4b9b10ba" />

!Map <img width="502" height="321" alt="map" src="https://github.com/user-attachments/assets/d534ba76-57d3-4d11-98eb-64159633c39d" />

## 🧠 Future enhancements
- API-based ingestion / scheduled refresh
- Forecasting project volumes by borough (Time series)
- GIS integration (ArcGIS visuals)
- Cross-city comparative dashboards (Austin/Chicago/Seattle)

## 👤 Authors
- Ravi Teja — Data Analyst (Volunteer)
