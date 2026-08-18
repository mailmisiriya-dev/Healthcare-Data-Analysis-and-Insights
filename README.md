# Healthcare Data Analysis & Insights — Excel

## Project Overview

This project focuses on analyzing healthcare and hospitalization data using **Microsoft Excel**. The objective is to clean, transform, combine, and analyze healthcare-related datasets to identify meaningful patterns in patient health conditions, hospitalization charges, demographics, and healthcare risk factors.

The project demonstrates practical **Excel data analytics skills**, including data cleaning, transformation, lookup functions, Pivot Tables, KPI analysis, and interactive dashboard development.

The final analysis combines information from customer profiles, medical examinations, and hospitalization records into a consolidated healthcare dataset for further analysis and visualization.

---

##  Project Objectives

The main objectives of this project are to:

* Clean and standardize raw healthcare data.
* Combine multiple healthcare-related datasets using Customer ID.
* Analyze patient health indicators such as BMI and HbA1c.
* Identify diabetes and weight-status patterns.
* Analyze smoking and heart-related health conditions.
* Examine hospitalization charges.
* Compare healthcare costs across hospital and city tiers.
* Analyze patient age and demographic patterns.
* Create Pivot Tables for summarized analysis.
* Develop an interactive Excel dashboard.
* Generate meaningful healthcare insights to support data-driven decision-making.

---

##  Dataset Structure

The Excel workbook contains the following sheets:

### 1. Customer Names

Contains customer identification and name-related information.

**Key columns:**

* Customer ID
* Name
* Title
* First Name
* Last Name

**Records:** 2,335 customers

---

### 2. Medical Examinations

Contains patient medical examination and health-condition information.

**Key columns:**

* Customer ID
* BMI
* HbA1c
* Heart Issues
* Any Transplants
* Cancer History
* Number of Major Surgeries
* Smoker
* Cleaned Smoker
* Cleaned Heart Issues
* Cleaned Number of Major Surgeries
* Weight Status
* Diabetes Status

This sheet was used to standardize inconsistent categorical values and create analytical health-status fields.

---

### 3. Hospitalisation Details

Contains hospitalization, demographic, location, and healthcare-charge information.

**Key columns:**

* Customer ID
* Year
* Month
* Date
* Children
* Charges
* Hospital Tier
* City Tier
* State ID
* Date of Birth
* Age

Additional cleaned columns were created for standardized dates, years, hospital tiers, city tiers, and state IDs.

---

### 4. Healthcare

This is the **consolidated analytical dataset** created by combining relevant information from the different source sheets.

It contains health, demographic, hospitalization, and cost-related variables.

**Key columns include:**

* Customer ID
* First Name
* BMI
* HbA1c
* Heart Issues
* Any Transplants
* Cancer History
* Number of Major Surgeries
* Smoker
* Weight Status
* Diabetes Status
* Date of Birth
* Charges
* Hospital Tier
* City Tier
* State ID
* Age

**Records:** 2,335 customers

This consolidated dataset forms the main basis for the analysis and dashboard.


# Data Cleaning & Transformation

Data preparation was an important part of this project.

The following Excel techniques were used:

### Data Cleaning

* Removed unnecessary spaces and inconsistent text values.
* Standardized categorical values such as Yes/No and smoker status.
* Converted inconsistent values into standardized categories.
* Converted dates into proper Excel date formats.
* Converted numerical fields into appropriate numeric data types.
* Created cleaned versions of important columns.
* Checked data consistency before analysis.

### Derived Columns

Additional analytical fields were created, including:

* **Weight Status**
* **Diabetes Status**
* **Age**
* **Cleaned Smoker**
* **Cleaned Heart Issues**
* **Cleaned Number of Major Surgeries**
* **Cleaned Hospital Tier**
* **Cleaned City Tier**
* **Cleaned State ID**

---

#  Data Integration

Multiple worksheets were combined using **Customer ID** as the primary matching field.

The integration process connected:

**Customer Information → Medical Examination Data → Hospitalization Data → Consolidated Healthcare Dataset**

This created a single analytical view that allows health conditions to be compared with hospitalization charges and demographic factors.

---

#  Excel Skills & Techniques Used

## Excel Functions

The project demonstrates the use of Excel functions and features such as:

* `XLOOKUP`
* `VLOOKUP`
* `SUMIF`
* `SUMIFS`
* `COUNTIF`
* `COUNTIFS`
* `TRIM`
* `PROPER`
* `IF`
* `IFERROR`
* Date functions
* Text functions
* Logical functions

---

## Pivot Tables

Pivot Tables were used to summarize large amounts of healthcare data and identify patterns across different dimensions.

Examples include:

* Average healthcare charges by hospital tier
* Patient count by diabetes status
* Patient count by weight status
* Charges by city tier
* Patient distribution by age
* Health condition analysis
* Smoking status analysis

---

##  Data Visualization

Different Excel charts were used to communicate healthcare insights effectively.

Potential analytical visualizations include:

* KPI cards
* Column charts
* Bar charts
* Pie/Doughnut charts
* Distribution charts
* Comparison charts
* Healthcare charge analysis

The dashboard combines these visualizations into a single analytical view.

---

# 📈 Key KPIs

The project focuses on important healthcare KPIs such as:

* **Total Patients**
* **Average Age**
* **Average BMI**
* **Average HbA1c**
* **Total Hospitalization Charges**
* **Average Hospitalization Charges**
* **Diabetes Patients**
* **Obesity Patients**
* **Smokers**
* **Patients with Heart Issues**
* **Patients with Cancer History**
* **Patients with Major Surgeries**

These KPIs provide a high-level overview of the healthcare population and associated costs.

---

# 🔍 Key Areas of Analysis

### 1. Patient Demographics

The analysis examines patient age and demographic characteristics to understand the composition of the healthcare population.

### 2. BMI & Weight Status

BMI values were analyzed to classify patients into different weight-status categories and identify the prevalence of obesity and other weight-related conditions.

### 3. Diabetes Analysis

HbA1c values were analyzed alongside the derived Diabetes Status field to understand diabetes and prediabetes patterns.

### 4. Smoking Analysis

Smoking status was standardized and analyzed to identify the proportion of patients who smoke and explore its relationship with healthcare conditions and costs.

### 5. Heart Health

Heart-related conditions were analyzed to understand their distribution across the patient population.

### 6. Hospitalization Charges

Hospitalization charges were analyzed to identify cost patterns and compare expenses across different hospital and city tiers.

### 7. Hospital Tier Analysis

Hospitalization charges were compared across hospital tiers to identify differences in healthcare costs.

### 8. City Tier Analysis

The analysis examines healthcare charges across different city tiers.

### 9. Age Analysis

Patient age was calculated from date-of-birth information and used to identify age-related patterns in healthcare conditions and hospitalization costs.

---

# Business & Healthcare Insights

The project can help answer questions such as:

* Which health conditions are most common?
* What percentage of patients are diabetic or prediabetic?
* How common is obesity among patients?
* How does smoking status vary across the patient population?
* Which hospital tier has higher average hospitalization charges?
* Does city tier influence healthcare costs?
* Which age groups have higher healthcare expenses?
* Are certain health conditions associated with higher hospitalization charges?
* What are the major healthcare cost drivers?
* Which patient groups may require greater healthcare attention?

---

# 📊 Dashboard

The Excel dashboard provides a centralized view of the healthcare analysis.

### Dashboard Components

The dashboard includes:

* Healthcare KPIs
* Patient demographics
* Health-condition analysis
* Diabetes analysis
* Weight-status analysis
* Smoking analysis
* Hospitalization charge analysis
* Hospital tier comparison
* City tier comparison
* Interactive Pivot Table-based visualizations

The dashboard is designed to make healthcare trends easier to understand without manually analyzing the underlying dataset.

---

# 🧰 Tools & Technologies

| Tool                  | Purpose                                 |
| --------------------- | --------------------------------------- |
| **Microsoft Excel**   | Data cleaning, transformation, analysis |
| **Excel Functions**   | Data preparation and calculations       |
| **Pivot Tables**      | Data summarization                      |
| **Pivot Charts**      | Data visualization                      |
| **Excel Dashboard**   | Interactive reporting                   |
| **XLOOKUP / VLOOKUP** | Data integration                        |
| **SUMIFS / COUNTIFS** | KPI calculations                        |

---
