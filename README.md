# HR-Employee-Attrition-PowerBi
HR Employee Attrition Analysis using Power BI with IBM HR dataset, insights, DAX, and dashboard.
# HR Employee Attrition Analysis (Power BI)

##  Project Overview
This project analyzes employee attrition patterns using the IBM HR Analytics dataset.  
The goal is to identify key factors driving employee turnover and provide data-driven insights for HR decision-making.

This analysis is built in **Power BI**, using DAX, data modeling, and interactive visuals.

---

##  Dataset
- Source: IBM HR Analytics Employee Attrition & Performance dataset
- Format: CSV
- Records: 1,470 employees
- Target Column: **Attrition (Yes/No)**

---

## Objectives
- Analyze attrition based on **age, salary, job role, gender, education, work-life balance**.
- Identify **top factors influencing employee churn**.
- Build an interactive **Power BI HR analytics dashboard**.
- Provide **actionable insights & recommendations** for HR teams.

---

## 🛠 Tools & Technologies
- **Power BI Desktop**
- **DAX (Data Analysis Expressions)**
- **Power Query**
- Excel (optional)
- Git / GitHub

---

## Dashboard Features

### **KPIs**
- Total Employees    
- Attrition Rate (%)  

### **Key Visuals**
- Attrition by Age Group  
- Attrition by Monthly Income Band  
- Attrition by Job Role  
- Attrition by OverTime  
- Attrition by Job Satisfaction (Heatmap)  
- Employee demographic distribution  

### **Slicers**
- Department  
- Job Level   
- Gender  
- Marital Status  
---

##  DAX Measures Used

Income Band =
SWITCH(
    TRUE(),
    Employees[MonthlyIncome] < 5000, "Low",
    Employees[MonthlyIncome] < 10000, "Medium",
    "High"
)
