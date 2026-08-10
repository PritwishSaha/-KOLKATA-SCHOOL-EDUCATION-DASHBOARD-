# 🏫 Kolkata School Education Analytics Dashboard

<p align="center">
  <img src="Screenshot 2026-08-10 052014.png" alt="Kolkata School Education Dashboard" width="100%">
</p>

<p align="center">
  <b>Power BI Data Analytics Project</b>
</p>

<p align="center">

<img src="https://img.shields.io/badge/Power%20BI-Analytics-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"><img src="https://img.shields.io/badge/Power%20Query-Data%20Cleaning-217346?style=for-the-badge"><img src="https://img.shields.io/badge/DAX-Data%20Modeling-512BD4?style=for-the-badge"><img src="https://img.shields.io/badge/CSV-Dataset-1F6FEB?style=for-the-badge">

</p>

📌 Project Overview

The Kolkata School Education Analytics Dashboard is an interactivePower BI data analytics project developed to understand thedistribution of schools and students across Kolkata's boroughs andwards.

The project transforms raw school-level data into a visually interactivedashboard using Power Query, DAX, and Power BI.

It provides a consolidated view of:

🏫 School distribution

👨‍🎓 Student population

🏙️ Borough-level analysis

📍 Ward-level analysis

🏷️ School type/ownership

📊 Student-size classification

Project Focus: Descriptive analytics of Kolkata's school andstudent distribution.

🎯 Project Objectives

The main objectives of this project are to:

Analyze the total number of schools and students.

Compare school distribution across wards.

Compare student populations across boroughs.

Analyze student distribution by ward.

Understand school ownership/type.

Categorize schools according to student population.

Build an interactive and easy-to-understand Power BI dashboard.

Convert raw educational data into meaningful analytical insights.

📊 Dashboard at a Glance

Metric                          Value

🏫 Total Schools          259👨‍🎓 Total Students       ~28K🏙️ Boroughs Covered        15📍 Wards Covered          106

📈 Dashboard Features

🏫 1. Schools by Ward

Analyzes how schools are distributed across different municipal wardsand helps identify wards with relatively higher or lower numbers ofschools.

👨‍🎓 2. Students by Borough

Compares student populations across Kolkata's boroughs to identifydifferences in student concentration.

📊 3. School Distribution by Student Size

Schools are grouped into five student-population categories:

Category          Students

🟢 Very Small        0--50🔵 Small           51--100🟡 Medium         101--150🟠 Large          151--200🔴 Very Large         200+

📍 4. Students by Ward

Provides a ward-level comparison of student populations and helpsidentify differences in student concentration.

🏷️ 5. Schools by Type

Shows the distribution of schools according to ownership/type, includingOWNED and RENTED categories present in the dataset.

🗂️ Dataset

The project uses the following dataset:

Kolkata_Schools.csv

Dataset Columns

Column             Description

SL No            Serial numberBorough          Municipal borough identifierWard No          Municipal ward numberSchool Code      School identifier/codeSchool Address   School addressSchool Type      School type/ownershipClasses          Classes offeredNo of Students   Number of students

🧹 Data Preparation

The dataset was prepared and transformed using Power Query.

Main Data Preparation Steps

✔️ Corrected data types.

✔️ Cleaned text fields.

✔️ Checked missing and inconsistent values.

✔️ Kept School Code as text because it contains alphanumericcodes.

✔️ Prepared categorical columns for visualization.

✔️ Created a Student_Size classification.

✔️ Prepared the dataset for Power BI analysis.

🧮 DAX Measures

Total Schools

Total Schools =
DISTINCTCOUNT(Kolkata_Schools[School Code])

Total Students

Total Students =
SUM(Kolkata_Schools[No of Students])

Total Boroughs

Total Boroughs =
DISTINCTCOUNT(Kolkata_Schools[Borough])

Total Wards

Total Wards =
DISTINCTCOUNT(Kolkata_Schools[Ward No])

Average Students per School

Average Students per School =
DIVIDE(
    [Total Students],
    [Total Schools]
)

🔍 Key Insights

The current dashboard provides the following high-level insights:

🏫 259 schools are represented in the dataset.

👨‍🎓 Approximately 28K students are represented.

🏙️ The dataset covers 15 boroughs.

📍 The dataset covers 106 wards.

📊 School distribution varies across wards.

👨‍🎓 Student populations vary across boroughs and wards.

🏫 Schools can be grouped according to their student population.

🏷️ Both OWNED and RENTED school types are represented.

Note: These are descriptive findings from the current dataset andshould not be interpreted as evidence of school overcrowding oreducation quality.

🛠️ Tech Stack

Technology           Purpose

📊 Power BI      Dashboard & data visualization🧹 Power Query   Data cleaning & transformation🧮 DAX           Measures & calculations📄 CSV           Source dataset

🔄 Project Workflow

Raw CSV Dataset
       │
       ▼
┌───────────────────┐
│    Power Query    │
│ Cleaning &        │
│ Transformation    │
└─────────┬─────────┘
          │
          ▼
┌───────────────────┐
│       DAX         │
│ Measures &        │
│ Calculations      │
└─────────┬─────────┘
          │
          ▼
┌───────────────────┐
│     Power BI      │
│ Visualization &   │
│ Interactive Report│
└─────────┬─────────┘
          │
          ▼
   📊 Final Dashboard

📁 Project Structure

Kolkata-School-Education-Analytics/
│
├── 📄 README.md
├── 📄 PROJECT_REPORT.txt
├── 📄 Kolkata_Schools.csv
│
├── 📊 dashboard/
│   └── Kolkata_School_Dashboard.pbix
│
└── 🖼️ images/
    └── dashboard.png

⚠️ Limitations

This project is a descriptive analytics dashboard, not a real-timeeducation monitoring system.

The current dataset does not contain:

❌ Teacher information

❌ Classroom capacity

❌ Historical enrollment data

❌ Ward population data

❌ School performance indicators

❌ Reliable school latitude/longitude coordinates

Therefore, the dashboard cannot independently determine whether aschool or ward is overcrowded.

Additional capacity, teacher, demographic, and historical data would berequired for that type of analysis.

🚀 Future Scope

The project can be expanded into a more advanced education analyticssystem by adding:

📈 Historical Analysis

Analyze year-over-year changes in student enrollment.

👨‍🏫 Teacher Analysis

Add teacher data and calculate student-to-teacher ratios.

🏫 Infrastructure Analysis

Add classroom and infrastructure data to study capacity and facilities.

🏙️ Population Analysis

Combine ward population data with school/student data.

🗺️ Geographic Analysis

Add reliable ward boundaries or school coordinates for geographicvisualization.

🔄 Automated Data Refresh

Connect the dashboard to a database or API for regularly refreshed data.

🤖 Machine Learning

Build a student-demand prediction model using historical enrollment anddemographic data.

📄 Project Report

A detailed project report is available here:

PROJECT_REPORT.txt

It contains:

Abstract

Introduction

Problem Statement

Objectives

Dataset Description

Data Preparation

DAX Measures

Dashboard Analysis

Key Findings

Use Case

Limitations

Future Scope

Conclusion

💡 What This Project Demonstrates

This project demonstrates practical skills in:

✔ Data Cleaning
✔ Data Transformation
✔ Exploratory Data Analysis
✔ Power Query
✔ DAX
✔ KPI Development
✔ Data Visualization
✔ Dashboard Design
✔ Business/Domain Analysis
✔ Analytical Storytelling

👨‍💻 Author

Pritwish Saha

B.Tech CSE (AI & ML) Student

Interested in:

Data Analytics • Machine Learning • Artificial Intelligence •Power BI

⭐ Support

If you find this project useful or interesting, consider giving therepository a ⭐ Star.

<p align="center">

<b>{=html}Built with Power BI 📊 | Data → Insights →Decisions</b>{=html}

</p>
