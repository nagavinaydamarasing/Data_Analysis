# Power BI End-to-End Project: Reimbursement Analysis

## 📌 Overview
This project analyzes employee reimbursement claims across multiple currencies. 
It demonstrates data cleaning in Power Query, DAX measures, and visualization best practices.

---

## 📂 Dataset Details
Columns included:
- **Employee_Name**  
- **Project**  
- **Expense_Type**  
- **Amount**  
- **Currency**  
- **Date**  

---

## 🛠️ Data Cleaning in Power Query
- Fixed spelling errors in `Expense_Type` column (Transportation, Miscellaneous, etc.)  
- Standardized project names (`ProjectA` → `Project_A`)  
- Imputed missing `Currency` values based on `Amount` column using custom rules  
- Created `Amount_INR` column with conversion logic:  
  - USD → 83  
  - EURO → 89.5  

---

## 📊 DAX Measures
- `Total_Reimbursement = SUM(Amount_INR)`  
- `Avg_Reimbursement = AVERAGE(Amount_INR)`  
- `Max_Reimbursement = MAX(Amount_INR)`  

---

## 📈 Visualizations
- Bar chart → Reimbursement by Project  
- Pie chart → Distribution by Expense Type  
- KPI cards → Total, Average, Max Reimbursement  

---

## 🚀 How to Use
1. Open the `.pbix` file in Power BI Desktop  
2. Explore dataset transformations in Power Query  
3. Review DAX measures under the Data tab  
4. Interact with dashboards for insights  

---

## 🔧 Modifications / Improvements
- Expanded expense categories for better grouping  
- Added slicers for filtering by Project and Employee  
- Improved currency conversion with parameterized values  
