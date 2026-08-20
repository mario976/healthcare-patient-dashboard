# Healthcare Patient Analytics Dashboard

An interactive Power BI dashboard analyzing 55,500+ hospital admission records to surface trends in patient demographics, billing, clinical outcomes, and operational load.

![Dashboard Preview](Dashboard Screenshot.png)

## Overview

Hospitals generate huge volumes of admissions, billing, and clinical data — but raw records rarely translate into decisions on their own. This project takes a raw patient admissions dataset and turns it into a self-service analytics dashboard that lets stakeholders explore patient demographics, insurance mix, prescribed medications, and cost trends without touching a spreadsheet.

**Key metrics tracked:**
- Total Patients & Admissions
- Average Length of Stay
- Average Billing Amount
- Room Utilization
- Top Prescribed Medications
- Insurance Provider Mix
- Admissions by Age Group, Gender, Blood Type, and Medical Condition

## Process

1. **Data Cleaning (Excel)** — Cleaned and validated the raw dataset: standardized date formats, checked for duplicate/inconsistent entries, and prepared the file for a stable load into Power BI.
2. **Data Modeling (Power BI / Power Query)** — Built calculated columns (e.g., Age Group bins) and confirmed data types for reliable time intelligence and filtering.
3. **DAX Measures** — Wrote a dedicated measures table (Total Patients, Total Admissions, Average Billing, Emergency Admissions %, Length of Stay, and ranking logic for Top 5 Medications) to keep the model clean and reusable.
4. **Dashboard Design** — Designed a single-page dashboard with a custom color theme, KPI summary row, dynamic field-parameter buttons (switch the demographic breakdown between Age Group / Blood Type / Medical Condition on the same chart), and a date-range slicer for time filtering.

## Key Insights

- The dataset covers **40,235 unique patients** across **55,500 total admissions** between 2019–2024.
- Average length of stay sits at **17.84 days**, with variation across medical conditions worth further investigation for capacity planning.
- Average billing per admission is **$21,835**, with insurance coverage fairly evenly split across the four major providers (~20% each) — no single provider dominates the patient base.
- **Seniors and middle-aged patients** account for the highest admission volumes by a clear margin over younger age groups, which has direct implications for staffing and resource allocation.
- The top prescribed medications (Metformin, Zanamivir, Methotrexate, Glipizide, Orlistat) suggest a patient population with a notable concentration of chronic/metabolic conditions.

## Tools Used

- **Microsoft Excel** — initial data cleaning and validation
- **Power BI Desktop** — data modeling, DAX, dashboard design
- **DAX** — custom measures, dynamic ranking (Top N), field parameters

## Files

- `Healthcare_Dashboard.pbix` — full Power BI report (open with Power BI Desktop)
- `dashboard_screenshot.png` — static preview of the dashboard
- `/data` — dataset used (raw and cleaned versions, if shared)

## Notes

This project uses a synthetic/sample healthcare dataset for analytics practice and portfolio purposes. It does not represent real patient data.

---

**Author:** Mario Fahim
