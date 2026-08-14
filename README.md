# Healthcare Appointment Attendance Analysis

## Project Overview

This project analyzes patient appointment attendance data to identify patterns in attendance and no-show behavior.

The analysis focuses on appointment attendance, patient demographics, health conditions, SMS reminders, waiting time, weekdays, age groups, gender, and neighbourhoods.

The main goal is to understand which factors may be associated with missed medical appointments and to present the findings through an interactive dashboard created in Google Sheets.

---

## Dataset

The dataset contains information about scheduled medical appointments, patients, and appointment attendance.

### Main variables

| Variable | Description |
|---|---|
| PatientID | Unique patient identifier |
| AppointmentID | Unique appointment identifier |
| Gender | Patient gender |
| ScheduledDay | Date when the appointment was scheduled |
| AppointmentDay | Date of the appointment |
| Age | Patient age |
| Neighbourhood | Patient's neighbourhood |
| Hypertension | Whether the patient has hypertension |
| Diabetes | Whether the patient has diabetes |
| ARI | Acute respiratory infection |
| SMS_received | Whether the patient received an SMS reminder |
| No_show | Whether the patient missed the appointment |
| Age_Group | Whether the patient belongs to the 65+ age group |
| Waiting_Days | Number of days between scheduling and appointment |
| Weekday | Day of the week of the appointment |

### No-show definition

For this analysis:

- `No_show = No` → patient **attended the appointment**
- `No_show = Yes` → patient **did not attend the appointment**

---

## Tools

- **Google Sheets** — data analysis, calculations, pivot tables, and dashboard creation
- **GitHub** — project documentation and version control

---

## Analysis Period

The analyzed appointments cover the period from **January 4, 2024 to July 24, 2024**.

---

# Key Performance Indicators

| KPI | Result |
|---|---:|
| Total Appointments | 1,000 |
| Unique Patients | 1,000 |
| Completed Visits | 828 |
| No-show Visits | 172 |
| Attendance Rate | 83% |
| No-show Rate | 17% |
| Average Waiting Days | 15 |

The overall attendance rate was **83%**, while **17% of scheduled appointments were missed**.

The average waiting time between scheduling and the appointment was **15 days**.

---

# Patient Age Statistics

| Metric | Value |
|---|---:|
| Average Age | 45 |
| Median Age | 45 |
| Minimum Age | 0 |
| Maximum Age | 90 |

The average and median patient age are both **45 years**, indicating that the age distribution is relatively balanced and not strongly skewed.

Patients in the dataset ranged from **0 to 90 years old**.

---

# Patient Health Conditions

| Health Condition | Quantity | % of Patients |
|---|---:|---:|
| Diabetes | 118 | 11.8% |
| Hypertension | 242 | 24.2% |
| ARI | 59 | 5.9% |


Among the analyzed health-related characteristics, **Hypertension status represented the largest group**, with 242 recorded cases (24.2%).

---

# SMS Reminder Analysis

SMS reminders were analyzed to determine whether receiving a reminder was associated with appointment attendance.

### No-show

| SMS Status | No-show | No-show Rate |
|---|---:|---:|
| SMS received | 95 | 16% |
| SMS not received | 77 | 19% |

### Attendance

| SMS Status | Attended | Attendance Rate |
|---|---:|---:|
| SMS received | 496 | 84% |
| SMS not received | 332 | 81% |

Patients who received SMS reminders had a **higher attendance rate (84%)** compared with patients who did not receive reminders (81%).

The no-show rate was also lower among patients who received SMS reminders:

- SMS received: **16% no-show**
- SMS not received: **19% no-show**

This suggests a possible positive association between SMS reminders and appointment attendance.

---

# No-show Analysis by Gender

| Gender | No-show Count | Share of No-shows |
|---|---:|---:|
| Female | 85 | 49% |
| Male | 87 | 51% |
| **Total** | **172** | **100%** |

Among all missed appointments, males accounted for **51%** and females for **49%**.

The difference between the two groups is relatively small.

---

# No-show Analysis by Age Group

| Age Group | No-show Count | Share of No-shows |
|---|---:|---:|
| 65+ | 45 | 26% |
| 0–18 | 37 | 22% |
| 51–65 | 32 | 19% |
| 19–35 | 30 | 17% |
| 36–50 | 28 | 16% |
| **Total** | **172** | **100%** |

The **65+ age group accounted for the largest share of no-shows (26%)**, followed by patients aged 0–18 (22%).

The 36–50 age group had the smallest share of no-shows among the defined age groups (16%).

---

# No-show Analysis by Neighbourhood

| Neighbourhood | No-show Count | Share of No-shows |
|---|---:|---:|
| Jardim | 40 | 23% |
| Centro | 37 | 22% |
| Santa Maria | 36 | 21% |
| Boa Vista | 32 | 19% |
| Industrial | 27 | 16% |
| **Total** | **172** | **100%** |

The highest number of missed appointments was recorded among patients from **Jardim**, with 40 no-shows (23% of all missed appointments).

Centro and Santa Maria followed with 22% and 21%, respectively.

---

# Appointment Attendance by Weekday

### Completed appointments

| Weekday | Completed Visits |
|---|---:|
| Monday | 124 |
| Tuesday | 114 |
| Wednesday | 106 |
| Thursday | 115 |
| Friday | 115 |
| Saturday | 115 |
| Sunday | 139 |
| **Total** | **828** |

The highest number of completed appointments occurred on **Sunday — 139 visits**.

### No-show appointments

| Weekday | No-show Count | Share of No-shows |
|---|---:|---:|
| Monday | 17 | 10% |
| Tuesday | 28 | 16% |
| Wednesday | 30 | 17% |
| Thursday | 20 | 12% |
| Friday | 29 | 17% |
| Saturday | 25 | 15% |
| Sunday | 23 | 13% |
| **Total** | **172** | **100%** |

The highest number of no-shows occurred on **Wednesday and Friday**, with 30 and 29 missed appointments respectively.

---

# Dashboard

The project includes a Google Sheets dashboard designed to provide a concise overview of appointment attendance and no-show behavior.

### Dashboard includes:

- Total appointments
- No-show rate
- No-show Visits
- Average waiting days
- Completed Visits
- Monthly Visit Trend
- No-show rate by sms-reminder
- No-show by neighbourhood
- No-show by age group
- No-show by weekday
- No-Show Rate vs. Waiting Time

The dashboard is designed to make the main patterns and differences easy to identify without reviewing the raw dataset.

---

# Key Insights

### 1. Overall attendance

The dataset contains **1,000 appointments**, of which **828 were completed** and **172 were missed**.

The overall attendance rate was **83%**, with a **17% no-show rate**.

### 2. SMS reminders

Patients who received SMS reminders had a slightly higher attendance rate (**84%**) than those who did not receive reminders (**81%**).

The no-show rate was correspondingly lower among patients who received SMS reminders (**16% vs. 19%**).

### 3. Age

The **65+ age group had the largest share of no-shows (26%)**.

This may indicate that older patients could require additional attention when designing appointment reminder or follow-up strategies.

### 4. Gender

No-shows were relatively evenly distributed by gender:

- Male — 51%
- Female — 49%

There is therefore no substantial difference in the composition of missed appointments by gender in this dataset.

### 5. Neighbourhood

**Jardim** had the largest share of no-shows among the analysed neighbourhoods (23%).

This may help identify areas where additional investigation or targeted communication could be useful.

### 6. Weekday

The largest number of completed visits occurred on **Sunday (139)**.

The largest number of missed appointments occurred on **Wednesday (30)**, closely followed by **Friday (29)**.

### 7. No-Show Rate vs. Waiting Time

There is a very weak positive correlation between waiting time and patient no-shows (r ≈ 0.04), suggesting that longer waiting times are associated with a slightly higher no-show rate. However, the relationship is too weak to consider waiting time a strong predictor of patient no-shows.

----
# Business Recommendations

Based on the analysis, several areas could be considered for further investigation:

1. **Continue using SMS reminders**, as patients who received reminders showed a slightly higher attendance rate.

2. **Pay additional attention to older patients**, particularly the 65+ group, which represented the largest share of no-shows.

3. **Investigate weekday patterns**, especially Wednesday and Friday, to determine whether scheduling patterns or operational factors contribute to missed appointments.

4. **Explore neighbourhood-level differences** to understand whether accessibility, transportation, or other local factors may influence attendance.

5. **Analyze waiting time in more detail** . The business should monitor and minimise excessive waiting times where possible, but should not rely on waiting time as a primary strategy for reducing no-shows, as the correlation is very weak. Further analysis of other factors is recommended to identify stronger predictors of patient no-shows and support more targeted business decisions.

---

# Limitations

The analysis describes patterns observed in the dataset but does not establish causal relationships.

For example, the lower no-show rate among patients receiving SMS reminders does not necessarily mean that SMS reminders directly caused patients to attend their appointments.

Additional variables and statistical analysis would be required to identify causal relationships.

The dataset also contains a limited number of appointments, so the results should not automatically be generalized to other healthcare settings or populations.

