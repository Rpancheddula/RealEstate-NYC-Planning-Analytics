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
![Summary & Boroughs](dashboard/images/summary_boroughs.png)
![Status & Year](dashboard/images/status_year.png)
![Monthly Trend](dashboard/images/monthly_trend.png)
![Top Admins](dashboard/images/top_admins.png)
![Map](dashboard/images/map.png)

## 🧠 Future enhancements
- API-based ingestion / scheduled refresh
- Forecasting project volumes by borough (Time series)
- GIS integration (ArcGIS visuals)
- Cross-city comparative dashboards (Austin/Chicago/Seattle)

## 👤 Authors
- Ravi Teja — Data Analyst (Volunteer)
