# Healthcare-Appointment-Analytics-
Project Overview

This project analyzes healthcare appointment data to identify patterns in:

Appointment attendance and no-shows
Patient demographics
Waiting time
Health conditions
SMS reminder effectiveness

The project was completed as a Test Assignment Simulation and includes data profiling, validation, cleaning, and exploratory analysis.

Dataset
Parameter	Description
Dataset	Healthcare Appointment Analytics
Source	Kaggle
Format	CSV
Storage	Local
Updates	No planned updates
Analysis Period	January 4, 2023 – July 23, 2023
Data Profiling

Before analysis, the dataset was checked for data quality issues.

Metric	Result
Rows	1,000
Columns	16
Missing Values	0
Missing Values %	0%
Duplicate AppointmentID	None
Negative Age Values	None

The dataset was validated, cleaned, and prepared for further analysis.

Key Metrics
Metric	Value
Total Appointments	1,001
Unique Patients	1,001
Attendance Rate	82.72%
No-show Rate	17.18%
Average Waiting Time	15 days
Key Findings
82.72% of appointments were attended.
17.18% of appointments resulted in a no-show.
The average waiting time between scheduling and appointment was 15 days.
Patient Age Analysis
Metric	Value
Average Age	45
Median Age	45
Minimum Age	0
Maximum Age	90

The average and median age are both 45 years, suggesting a relatively balanced age distribution.

Health Conditions
Condition	Patients	Percentage
Diabetes	118	8.5%
Hypertension	242	17.5%
Alcoholism	59	4.3%
Handicap	642	46.4%
Key Finding

Handicap was the most frequently recorded condition, representing 46.4% of patients in the analyzed dataset.

SMS Reminder Analysis

SMS reminders were analyzed to determine their relationship with appointment attendance.

Attendance Rate
SMS Status	Attended	Attendance Rate
SMS received	496	84%
SMS not received	332	81%
No-show Rate
SMS Status	No-shows	No-show Rate
SMS received	95	16%
SMS not received	77	19%
Key Finding

Patients who received SMS reminders had:

84% attendance rate compared with 81% for patients who did not receive SMS.
16% no-show rate compared with 19% for patients who did not receive SMS.

This indicates a positive association between SMS reminders and appointment attendance. However, the analysis does not prove that SMS reminders directly caused the improvement.

Business Insights
Appointment attendance is relatively high at 82.72%.
Approximately 17% of appointments are missed, making no-shows an important operational issue.
Patients receiving SMS reminders show a 3 percentage-point higher attendance rate.
The average waiting time is 15 days, which could be an important factor in future no-show analysis.
Patient demographics and health conditions provide opportunities for further patient segmentation.
No-show risk could be investigated using age, waiting time, health conditions, SMS reminders, and appointment characteristics.
Recommendations

Further analysis could include:

No-show rate by age group
No-show rate by waiting time
Attendance by health condition
SMS effectiveness by age group
Identification of high-risk patient segments
Healthcare appointment KPI dashboard
No-show prediction model
Tools & Technologies
CSV
SQL
Python / Pandas
Power BI / Tableau
GitHub
Project Structure
healthcare-appointment-analytics/
│
├── data/
│   └── healthcare_appointments.csv
│
├── analysis/
│   └── analysis.sql
│
├── dashboard/
│   └── healthcare_appointment_dashboard.pbix
│
└── README.md

Project Status

Completed — Test Assignment Simulation

The dataset was profiled, validated, cleaned, and analyzed. The analysis focuses on appointment attendance, no-shows, patient demographics, health conditions, waiting time, and SMS reminders.
