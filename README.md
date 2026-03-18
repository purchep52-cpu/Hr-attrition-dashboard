👥 HR Attrition Analysis Dashboard
IBM HR Analytics Dataset · Excel Pivot Tables + Slicers · 1,470 Employees
![Excel](https://img.shields.io/badge/Excel-Data%20Analysis-217346?style=flat&logo=microsoftexcel&logoColor=white)
![Pivot Tables](https://img.shields.io/badge/Pivot%20Tables-Slicers-217346?style=flat)
![Status](https://img.shields.io/badge/Status-Complete-22c55e?style=flat)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle%20IBM%20HR-20BEFF?style=flat&logo=kaggle&logoColor=white)
---
📌 Project Overview
This project analyzes 1,470 employee records from IBM's HR Analytics dataset to uncover the key drivers of employee attrition. Using Excel pivot tables, COUNTIFS formulas, and an interactive slicer dashboard, I identified actionable patterns that HR teams can use to reduce turnover and improve retention.
Business Question: Why are employees leaving - and what can the company do to stop it?
---
🔍 Key Findings
#	Finding	Impact
📌	Overall attrition rate: 16.1%	237 of 1,470 employees left
🔴	Overtime is the #1 driver	Overtime employees leave 3× more than non-overtime
📊	Sales department most at risk	20.63% attrition rate - highest of all departments
🏆	Sales Representatives have the highest role attrition	39.76% - nearly 4 in 10 leave
👶	Under 25 have the highest attrition of any age group	39.18% - early career employees are most at risk
😟	Low job satisfaction (score 1) has the highest attrition	22.84% - dissatisfaction drives exits
⏳	First 2 years are critical	35% attrition in early tenure - onboarding is key
💰	Low earners leave most	Leavers earn 30% less than stayers on average
---
💡 Recommendations
1. Cap Overtime Hours
Overtime is the single strongest predictor of attrition - overtime employees leave 3× more. Introduce flexible scheduling, compensatory time off, and workload redistribution to reduce dependency on overtime.
2. Review Sales Compensation
Sales Representatives have a 39.76% attrition rate - nearly 4 in 10 leave. Review commission structures, benchmark salaries against market rates, and reduce pressure targets to bring this number down.
3. Improve Onboarding of New Hires
35% of employees leave in their first 2 years. A structured onboarding programme with clear goals, regular check-ins, and a buddy system gives new hires the support they need to stay.
4. Create a Clear Career Path for Young Hires
Under 25s leave at 39.18% - the highest of any age group. Young employees leave when they can't see where they're going. A visible 1–3 year growth plan gives them a reason to stay.
5. Monthly Manager Check-ins
Regular 1-on-1s in the first year catch problems before they become resignation letters. Managers should meet every new hire monthly and document action points to show employees they are heard.
6. Salary Reviews for Low Earners
Leavers earn 30% less than stayers on average. Conduct a salary review for the bottom 25% of earners and introduce transparent pay bands so employees can see a clear path to higher earnings.
---
🗂 Dataset
Detail	Info
Source	IBM HR Analytics - Kaggle
Rows	1,470 employees
Columns	35 fields
Key fields	Attrition, Department, JobRole, Age, MonthlyIncome, OverTime, JobSatisfaction, YearsAtCompany, Gender
---
🛠 Tools Used
Tool	Purpose
Microsoft Excel	Pivot tables, COUNTIFS formulas, charts, slicers
Excel Pivot Tables	Attrition breakdowns by department, role, age, satisfaction
Excel Slicers	Interactive filtering by Department, Gender, OverTime
GitHub	Version control and portfolio publishing
---
📊 Sample Formula - Overtime Attrition Rate
The most important finding in this project - comparing attrition rates with and without overtime:
```excel
-- Attrition rate WITH overtime
=COUNTIFS(HRData[OverTime],"Yes",HRData[Attrition],"Yes")
/COUNTIF(HRData[OverTime],"Yes")

-- Attrition rate WITHOUT overtime
=COUNTIFS(HRData[OverTime],"No",HRData[Attrition],"Yes")
/COUNTIF(HRData[OverTime],"No")
```
👉 👉 [View full workbook — HR-Employee-Attrition.xlsx](./excel/HR-Employee-Attrition.xlsx)
---
📁 Repository Structure
```
hr-attrition-dashboard/
│ 
├── 📁 charts/
│   └── dashboard.pdf       #  dashboard screenshot
├── 📁 data/
├── 📁 excel/
    └── HR-Employee-Attrition.xlsx # Excel workbook - 3 sheets + charts
└── 📄 README.md                     # This file
```
---
📈 Excel Workbook Structure
Sheet	Contents
📋 Raw Data	IBM HR dataset - 1,470 rows, 35 columns
🔄 Pivot Tables	5 pivot tables - Dept, Job Role, Overtime, Age Group, Satisfaction
📈 Dashboard	KPI cards, 4 charts, slicers, findings + recommendations
---
🎛 Interactive Features
The dashboard includes 3 slicers that filter all charts simultaneously:
Department - Sales / R&D / Human Resources
Gender - Male / Female
OverTime - Yes / No
Click any slicer button and all 4 charts update instantly to show filtered results.
---
Analysis completed using Microsoft Excel · Dataset: IBM HR Analytics via Kaggle · 1,470 employees
