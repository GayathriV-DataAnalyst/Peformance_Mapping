# Employee Performance Mapping (SQL Project)

## 📌 Problem Statement
ScienceQtech is a startup working in the Data Science domain with projects in fraud detection, market basket analysis, self-driving cars, supply chain optimization, early detection of lung cancer, customer sentiment analysis, and drug discovery.  

With the annual appraisal cycle approaching, the HR department has requested reports on employee details, performance, and project involvement. The objective is to analyze employee data and generate insights for performance mapping, salary analysis, bonuses, and organizational improvements.

---

## 🎯 Objectives
- Generate employee performance reports for HR.  
- Find the maximum salary of employees.  
- Ensure job roles align with the organization’s standards.  
- Calculate bonuses to estimate extra expenses.  
- Provide insights to raise overall organizational performance.  

---

## 📂 Dataset Description
The project uses three CSV datasets that must be imported into a database named **`employee`**.

### 1. `emp_record_table`
Contains employee information:
- `EMP_ID` – Employee ID  
- `FIRST_NAME`, `LAST_NAME` – Employee names  
- `GENDER` – Gender  
- `ROLE` – Job role  
- `DEPT` – Department  
- `EXP` – Years of experience  
- `COUNTRY`, `CONTINENT` – Location details  
- `SALARY` – Salary  
- `EMP_RATING` – Performance rating  
- `MANAGER_ID` – Reporting manager ID  
- `PROJ_ID` – Assigned project  

### 2. `proj_table`
Contains project details:
- `PROJECT_ID` – Project ID  
- `PROJ_Name` – Project name  
- `DOMAIN` – Project domain  
- `START_DATE`, `CLOSURE_DATE` – Timeline  
- `DEV_QTR` – Scheduled quarter  
- `STATUS` – Current status  

### 3. `data_science_team`
Subset of employees in the Data Science team:
- `EMP_ID`, `FIRST_NAME`, `LAST_NAME`, `GENDER`  
- `ROLE`, `DEPT`, `EXP`, `COUNTRY`, `CONTINENT`  

---

## 📝 Tasks to Perform
1. Create a database named **`employee`** and import all datasets.  
2. Design an **ER diagram** for the database.  
3. Write SQL queries to:  
   - Fetch employee and department details.  
   - Filter employees by ratings (<2, >4, between 2–4).  
   - Concatenate names of employees in the Finance department.  
   - List managers and their number of reporters.  
   - Union employees from Healthcare and Finance departments.  
   - Group employees by department with max ratings.  
   - Find min & max salary per role.  
   - Rank employees by experience.  
   - Create a view for employees earning >6000.  
   - Retrieve employees with >10 years of experience (nested query).  
   - Create a stored procedure for employees with >3 years of experience.  
   - Implement a stored function to validate role standards:  
     - ≤2 yrs → Junior Data Scientist  
     - 2–5 yrs → Associate Data Scientist  
     - 5–10 yrs → Senior Data Scientist  
     - 10–12 yrs → Lead Data Scientist  
     - 12–16 yrs → Manager  
   - Create an index for faster search on employees named “Eric”.  
   - Calculate bonus = `5% of salary * employee rating`.  
   - Calculate average salary distribution per continent & country.  

---

## ⚙️ Deliverables
- SQL scripts for all queries, procedures, functions, and indexing.  
- ER diagram of the employee database.  
- Documentation (this README).  

---

## 🚀 Getting Started
1. Download the datasets from the LMS resource section.  
2. Import them into a database named **`employee`**.  
3. Execute SQL queries as per tasks above.  
