# HEALTHCARE ANALYTICS

## 📌 PROJECT OVERVIEW
This project focuses on analyzing healthcare operational, patient, doctor, appointment, treatment, and revenue data using SQL for data preparation and analysis and Power BI for interactive dashboards.
The goal is to derive actionable insights that support hospital management in decision-making, resource planning, and performance monitoring.

## 🎯 OBJECTIVES
   - ANALYZE PATIENT DEMOGRAPHICS AND VISIT BEHAVIOR
   - TRACK APPOINTMENT TRENDS AND COMPLETION RATES
   - EVALUATE DOCTOR AND DEPARTMENT PERFORMANCE
   - UNDERSTAND TREATMENT AND DIAGNOSIS PATTERNS
   - MEASURE REVENUE, BILLING, AND FINANCIAL KPIs

## 🗂️ DATASETS USED
The project uses multiple related tables to enable relational analysis:
   - <a href="https://github.com/Saranes55/SQL-PowerBI_Project/blob/main/Healthcare%20Analysis/Datasets/Patients.csv">**PATIENTS**</a> – Patient demographics (Age, Gender, City)
   - <a href="https://github.com/Saranes55/SQL-PowerBI_Project/blob/main/Healthcare%20Analysis/Datasets/Doctors.csv">**DOCTORS**</a> – Doctor details and departments
   - <a href="https://github.com/Saranes55/SQL-PowerBI_Project/blob/main/Healthcare%20Analysis/Datasets/Appointments.csv">**APPOINTMENTS**</a> – Appointment dates, status, doctor & patient mapping
   - <a href="https://github.com/Saranes55/SQL-PowerBI_Project/blob/main/Healthcare%20Analysis/Datasets/Treatment.csv">**TREATMENTS**</a> – Diagnosis and treatment information
   - <a href="https://github.com/Saranes55/SQL-PowerBI_Project/blob/main/Healthcare%20Analysis/Datasets/Billing.csv">**BILLING**</a> – Treatment cost, revenue, and payment status

## 🧹 DATA CLEANING & PREPARATION (SQL)
Key data preparation steps performed using SQL:
   - NULL VALUE CHECKS AND REMOVAL
   - INVALID AGE AND DATE VALIDATION
   - DUPLICATE RECORD IDENTIFICATION
   - STANDARDIZATION OF COLUMNS (STATUS, GENDER, CITY)
   - DATA TYPE CORRECTIONS
   - RELATIONAL JOINS BETWEEN TABLES

## DASHBOARD OVERVIEW
![Screenshot (495)](https://github.com/Saranes55/SQL-PowerBI_Project/blob/main/Healthcare%20Analysis/Dashboard/Healthcare%20Overview.png)

## 🔍 KEY ANALYSIS QUESTIONS & 📊 POWER BI DASHBOARD DESIGN

## 👤 PATIENT ANALYSIS
   - TOTAL NUMBER OF PATIENTS
   - AVERAGE PATIENT AGE
   - AGE GROUP DISTRIBUTION
   - GENDER DISTRIBUTION
   - PATIENT COUNT BY CITY
   - TOP 10 FREQUENT VISITING PATIENTS
   - REPEAT VISIT RATE

![Screenshot (495)](https://github.com/Saranes55/SQL-PowerBI_Project/blob/main/Healthcare%20Analysis/Dashboard/Patients%20Analysis.png)

## 📅 APPOINTMENT ANALYSIS
   - TOTAL APPOINTMENTS
   - COMPLETION RATE
   - CANCELLING RATE
   - MONTHLY APPOINTMENT TREND
   - APPOINTMENTS BY DAY OF WEEK
   - APPOINTMENT STATUS DISTRIBUTION

![Screenshot (495)](https://github.com/Saranes55/SQL-PowerBI_Project/blob/main/Healthcare%20Analysis/Dashboard/Appointments%20Analysis.png)
  
## 🩺 DOCTOR ANALYSIS
   - TOTAL DOCTORS
   - AVERAGE REVENUE PER DOCTOR
   - AVERAGE APPOINTMENTS PER DOCTOR
   - APPOINTMENTS BY DOCTOR
   - REVENUE BY DOCTOR
   - DEPARTMENT-WISE DOCTORS

![Screenshot (495)](https://github.com/Saranes55/SQL-PowerBI_Project/blob/main/Healthcare%20Analysis/Dashboard/Doctor%20Performance.png)

## 💊 TREATMENT & DIAGNOSIS ANALYSIS
   - AVERAGE TREATMENT COST
   - REVENUE BY DIAGNOSIS
   - TREATMENTS ARE PROVIDED BY DIAGNOSIS 
   - AVERAGE TREATMENT COST BY DIAGNOSIS

![Screenshot (495)](https://github.com/Saranes55/SQL-PowerBI_Project/blob/main/Healthcare%20Analysis/Dashboard/Diagnosis%20Analysis.png)

## 💰 BILLING & REVENUE ANALYSIS
   - TOTAL REVENUE
   - AVERAGE REVENUE PER CITY
   - MONTHLY REVENUE TREND
   - REVENUE PER CITY
   - REVENUE BY PAYMENT MODES

![Screenshot (495)](https://github.com/Saranes55/SQL-PowerBI_Project/blob/main/Healthcare%20Analysis/Dashboard/Billing%20%26%20Rervenue.png)

## 🛠️ TOOLS & TECHNOLOGIES
   - SQL (MySQL) – Data cleaning, joins, aggregations, KPIs
   - Power BI – Data modeling, DAX, interactive dashboards

## HOW TO IMPORT SQL QUERIES INTO POWER BI

### STEP 1: OPEN POWER BI DESKTOP
   - LAUNCH POWER BI DESKTOP
   - CLICK HOME → GET DATA → MYSQL DATABASE
     (OR SQL SERVER DEPENDING ON YOUR DB)

### STEP 2: CONNECT TO DATABASE
- ENTER:
    - SERVER NAME
    - DATABASE NAME
- CLICK OK

### STEP 3: CHOOSE IMPORT MODE
- SELECT IMPORT
  
✔ FAST PERFORMANCE

✔ BEST FOR PORTFOLIO

### STEP 4: USE ADVANCED OPTIONS (IMPORTANT)
- EXPAND ADVANCED OPTIONS
- PASTE YOUR SQL QUERY IN:
  - SQL STATEMENT (OPTIONAL)
-  PASTE ONLY ONE FINAL QUERY AT A TIME

### STEP 5: LOAD OR TRANSFORM
- CLICK TRANSFORM DATA (RECOMMENDED)
- RENAME COLUMNS
- SET DATA TYPES
- CLICK CLOSE & APPLY

## Project Structure

```
Healthcare-Analysis-SQL-PowerBI/
│
├── 01_Database_Setup/
│   ├── create_database.sql
│   ├── create_tables.sql
│   └── insert_data.sql
│
├── 02_Data_Cleaning/
│   ├── 01_check_null_values.sql
│   ├── 02_remove_duplicates.sql
│   ├── 03_validate_age_data.sql
│   ├── 04_standardize_gender_city.sql
│   └── 05_data_quality_checks.sql

│
├── 03_executive_overview/
│   ├── 01_total_revenue.sql
│   ├── 02_total_patients.sql
│   ├── 03_total_doctors.sql
│   ├── 04_average_bill_amount.sql
│   └── 05_total_appointments.sql
│   ├── 06_department_by_revanue.sql
│   ├── 07_monthly_revenue_trends.sql
│   ├── 08_appointment_status.sql
│   └── 09_monthly_appointment_trend.sql
│
├── 03_Patient_Analysis/
│   ├── 01_total_patients.sql
│   ├── 02_average_patient_age.sql
│   ├── 03_age_group_distribution.sql
│   ├── 04_gender_distribution.sql
│   ├── 05_patient_count_by_city.sql
│   ├── 06_top_10_frequent_patients.sql
│   └── 07_repeat_visit_rate.sql
│
├── 04_Appointment_Analysis/
│   ├── 01_total_appointments.sql
│   ├── 02_monthly_appointment_trend.sql
│   ├── 03_appointments_by_day_of_week.sql
│   ├── 04_appointment_status_distribution.sql
│   ├── 05_completion_rate.sql
│   └── 06_cancellation_rate.sql
│
├── 05_Doctor_Department_Analysis/
│   ├── 01_total_doctors.sql
│   ├── 02_average_appointmnet_per_doctor.sql
│   ├── 03_average_revenue_per_doctor.sql
│   ├── 04_.revenue_by_doctor.sql
│   └── 05_department_doctors.sql
│
├── 06_Treatment_Diagnosis_Analysis/
│   ├── 01_average_treatment_cost.sql
│   ├── 02_treatments_per_diagnosis.sql
│   ├── 03_revenue_by_diagnosis.sql
│   └── 04_average_treatment_cost_by_diagnosis.sql
│
├── 07_Billing_revenue_Analysis/
│   ├── 01_total_revenue.sql
│   ├── 02_monthly_revenue_trend.sql
│   ├── 03_average_revenue_per_city.sql
│   ├── 04_revenue_by_payment_mode.sql
│   └── 05_revenue_by_city.sql
│
├── 08_PowerBI_Queries/
│   ├── executive_overview.sql
│   ├── patient_dashboard.sql
│   ├── appointment_dashboard.sql
│   ├── doctor_dashboard.sql
│   ├── treatment_dashboard.sql
│   └── revenue_dashboard.sql
│
│
└──  README.md

```

## ✅ CONCLUSION

This healthcare analytics project demonstrates end-to-end data analysis skills, from SQL-based data cleaning and querying to Power BI dashboard development.
The insights generated can help hospitals improve patient care, doctor utilization, and financial performance.






















