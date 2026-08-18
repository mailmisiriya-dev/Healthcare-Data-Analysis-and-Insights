# Healthcare-Data-Analysis-and-Insights
Excel project analyzing patient health and hospitalization data, data cleaning, transformation, pivot tables, and an interactive dashboard with slicers.

Healthcare Data Analysis & Insights — Excel
About This Project
This project analyzes a healthcare dataset spanning medical examinations, hospitalization records, and customer profiles, using Excel to clean, transform, and combine the data into a single analytical view. The goal is to surface relationships between patient health metrics — BMI, HbA1C, smoking, transplant history — and healthcare costs, then present them through an interactive dashboard.

Problem Statement
Healthcare providers and policymakers generate vast amounts of patient data daily, but raw data alone doesn't drive better decisions. This project cleans and consolidates medical examination, hospitalization, and customer data to extract insights into patient health profiles, medical histories, and healthcare costs — enabling more informed, data-backed decisions on patient care and cost management.

Dataset Summary
Property	Value
Source Tables	Customer Names, Medical Examinations, Hospitalisation Details
Combined Records	2,335 patients
Join Key	Customer ID (via VLOOKUP)
Final Sheet	"Healthcare" — 17 consolidated columns
Stage 1 — Data Cleaning
Missing value audit: Counted values marked ? across the Medical Examinations and Hospitalisation Details tables
Month/Year imputation: Missing month filled with "Sep"; missing year filled with the average year, rounded to the nearest integer
Mode imputation: Missing smoker, Hospital tier, and City tier values filled with each column's most frequent value
State ID: Missing values handled with a fallback strategy (e.g. "Unknown") to avoid dropping records
Stage 2 — Data Transformation
Name splitting: names column split into Title, First Name, Last Name
Surgery count cleanup: NumberOfMajorSurgeries converted to fully numeric by replacing non-numeric characters with meaningful values
Consistency checks: Reviewed Heart Issues and smoker columns for inconsistent entries and corrected them
Weight Status (derived from BMI):
Below 18.5 → Underweight
18.5–24.9 → Normal Weight
25.0–29.9 → Overweight
30.0+ → Obesity
Diabetes Status (derived from HbA1C):
Below 5.7 → Normal
5.7–6.4 → Prediabetes
6.5+ → Diabetes
Date of Birth: year, month, date merged into one Date of Birth column, formatted DD-MMM-YYYY
Age: Calculated from Date of Birth relative to the dataset collection date (8 June 2023)
Charges: Formatted as currency ($)
Stage 3 — Consolidation, Analysis & Dashboard
Built a "Healthcare" sheet combining all three source tables via VLOOKUP on Customer ID, retaining the 17 key fields needed for analysis
Built PivotTables to drive each visualization
Pie/Donut charts:

Cancer history distribution among smokers vs. non-smokers
Major surgeries total and average HbA1C, split by transplant history
Column/Bar charts:

Healthcare charges by Weight Status and by Diabetes Status
Average charges by hospital tier, compared across states
Line/Scatter plots:

Age vs. BMI and Age vs. HbA1C correlation
Age vs. healthcare charges relationship
Interactive Dashboard:

Consolidates all six visualizations onto a single "HEALTHCARE DASHBOARD" sheet
Slicers for Weight Status and Diabetes Status filter all charts simultaneously, enabling cross-comparison of health outcomes and cost
Files in This Repository
File	Description
Healthcare_Analysis.xlsx	Final workbook — raw tables, cleaning/transformation, combined Healthcare sheet, PivotTables, and Dashboard
README.md	Project documentation
Tools Used
Tool	Role
Microsoft Excel	Data cleaning, transformation, formulas
VLOOKUP	Merging three source tables into one
PivotTables	Aggregating data for each chart
Excel Charts & Slicers	Visualization and interactive dashboard filtering
