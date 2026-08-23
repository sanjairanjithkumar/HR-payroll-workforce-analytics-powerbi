# HR Payroll & Workforce Analytics — Power BI Dashboard

Interactive Power BI dashboard analyzing employee, department, and payroll data, with five report pages covering an executive summary, employee demographics, payroll breakdowns, department comparisons, and employee-level drill-through.

---

## 📌 Overview

This Power BI report (`project_2.pbix`) models employee, department, and salary transaction data into a connected data model, giving HR stakeholders a single interactive tool to monitor headcount, payroll cost, and departmental pay trends — with the ability to drill into an individual employee's full salary history.

## 🎯 Objective

- Model employee, department, and salary data into a connected Power BI data model.
- Track core workforce KPIs: total employees, gender split, and department headcount.
- Track core payroll KPIs: total and average net salary, basic salary, bonus, commission, and deductions.
- Compare payroll cost and headcount across departments and locations.
- Monitor payroll and bonus trends over time (by month/quarter/year).
- Enable drill-through from summary views to individual employee salary history.

## 🗂️ Data Model

| Table | Type | Key Fields |
|---|---|---|
| **fact_salary_dataset** | Fact | EmployeeID, SalaryDate, BasicSalary, Bonus, Commission, Deductions, NetSalary |
| **employee_dataset** | Dimension | EmpID, EmpName, Gender, Designation |
| **dept_dataset** | Dimension | DeptName, Location |
| **Dim Calender** | Dimension (Date table) | Date, Year, Quarter, Month, Day — used for the date hierarchy across all pages |

## 🛠️ Tools & Tech Stack

- **Power BI Desktop** — data import, modeling, DAX measures, report design
- **Power Query Editor** — cleaning and shaping employee, department, and salary data
- **Data Model / Relationships View** — linking fact_salary_dataset to employee_dataset, dept_dataset, and Dim Calender
- **DAX** — measures for payroll totals/averages, headcount splits, and highest/lowest-paying department

## 📊 Report Pages

### Executive Dashboard
KPI cards (Total Net Salary, Average Net Salary, Total Basic Salary, Total Deductions, Total Bonus, Employee Count), net salary trend over time, Net Salary by Department, gender split, and headcount by Department.

### Employee Analysis
Headcount by Designation, gender split, headcount by Year, and a detail table of employees with gender, designation, bonus, commission, and net salary.

### Payroll Analysis
KPI cards for basic salary, HRA, allowances, bonus, commission, and deductions; monthly payroll breakdown and trend charts; payroll/bonus by department.

### Department Analysis
KPI cards highlighting the highest- and lowest-paying departments; average net salary, headcount, total payroll, bonus, and deductions broken down by department and location.

### Employee Drill-through
KPI cards for net salary, bonus, commission, and deductions; trend lines over time; and a detailed employee-level salary table for drilling into individual records.

## 💡 Key DAX Measures

Total/Average Net Salary, Total Basic Salary, Total HRA, Total Allowances, Total Bonus, Total Commission, Total Deductions, Total Payroll, Male/Female employee counts, and Highest/Lowest Paying Department.

## 👤 Author

Sanjai — Data Analytics student (Python with Data Analytics, QSpiders, Bengaluru)
