🏫 Kolkata School Education Analytics Dashboard

<p align="center">
  <img src="Screenshot 2026-08-10 052014.png" alt="Kolkata School Education Dashboard" width="100%">
</p>

<p align="center">
  <b>Power BI Data Analytics Project</b>
</p>

📌 Project Overview

The Kolkata School Education Analytics Dashboard is an interactivePower BI project that analyzes the distribution of schools and studentsacross Kolkata's boroughs and wards.

The project transforms raw school-level data into an interactivedashboard containing KPIs, comparative charts, student-size analysis,and school-type analysis.

🎯 Project Objectives

Analyze the total number of schools and students.

Compare schools across wards.

Compare student populations across boroughs.

Analyze student distribution by ward.

Analyze school ownership/type.

Categorize schools based on student population.

Build an interactive educational analytics dashboard.

📊 Dashboard KPIs

KPI

Value

🏫 Schools

259

👨‍🎓 Students

~28K

🏙️ Boroughs

15

📍 Wards

106

📈 Dashboard Visualizations

1. Schools by Ward

Shows how schools are distributed across different wards.

2. Students by Borough

Compares student populations across Kolkata's boroughs.

3. School Distribution by Student Size

Groups schools into:

Very Small: 0–50

Small: 51–100

Medium: 101–150

Large: 151–200

Very Large: 200+

4. Students by Ward

Shows differences in student population across wards.

5. Schools by Type

Shows the distribution of school types/ownership, including OWNEDand RENTED categories present in the dataset.

🗂️ Dataset

The dataset is stored in:

Kolkata_Schools.csv

Main Columns

Column

Description

SL No

Serial number

Borough

Municipal borough

Ward No

Municipal ward

School Code

School identifier

School Address

School address

School Type

School type/ownership

Classes

Classes offered

No of Students

Number of students

🧹 Data Preparation

The dataset was prepared using Power Query.

Main steps included:

Data type correction

Text cleaning

Checking missing/inconsistent values

Keeping School Code as text

Preparing categorical fields

Creating the Student_Size classification

🧮 DAX Measures

Total Schools =
DISTINCTCOUNT(Kolkata_Schools[School Code])

Total Students =
SUM(Kolkata_Schools[No of Students])

Total Boroughs =
DISTINCTCOUNT(Kolkata_Schools[Borough])

Total Wards =
DISTINCTCOUNT(Kolkata_Schools[Ward No])

Average Students per School =
DIVIDE([Total Students], [Total Schools])

🔍 Key Insights

The current dashboard shows:

259 schools represented in the dataset.

Approximately 28K students represented.

15 boroughs covered.

106 wards covered.

School distribution varies across wards.

Student populations vary across boroughs and wards.

Schools can be categorized according to student population.

Both OWNED and RENTED school types are represented.

🛠️ Tools & Technologies

Power BI — Dashboard and visualization

Power Query — Data cleaning and transformation

DAX — Measures and calculations

CSV — Source dataset

⚠️ Limitations

This project is a descriptive analytics dashboard, not a real-timeeducation monitoring system.

The current dataset does not contain:

Teacher information

Classroom capacity

Historical enrollment

Ward population

School performance indicators

Reliable school coordinates

Therefore, the dashboard should not be used alone to conclude that aschool or ward is overcrowded.

🚀 Future Scope

The project can be extended with:

Historical enrollment data

Teacher/student ratio analysis

Classroom capacity data

Ward population data

Geographic school/ward data

School infrastructure data

Automated database/API refresh

Student demand prediction using Machine Learning

📄 Full Project Report

For the detailed project documentation, see:

PROJECT_REPORT.txt

👨‍💻 Author

Pritwish Saha

B.Tech CSE (AI & ML) Student

⭐ If you find this project useful, consider giving the repository a star.
