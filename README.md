# OPERATIONS-TURN-AROUND-TIME-ANALYSIS
This project is a Power BI dashboard built to track and analyze Turnaround Time (TAT) for operational cases. It covers both completed and pending cases, helping identify performance gaps, SLA breaches, and workload distribution across executives.

## 📸 Dashboard Preview

### ✅ Completed Cases Analysis
![Completed](images/completed-dashboard.png)

### ⏳ Pending Cases Tracking
![Pending](images/pending-dashboard.png)

## 🎯 Project Objective

The goal of this dashboard is to:

- Track case completion performance  
- Compare **Achieved TAT vs Target TAT**  
- Identify SLA breaches  
- Monitor pending workload and aging  
- Evaluate employee performance  
- Provide service-level insights  

## 📊 Key Insights Delivered

### ✅ Completed Cases

- Total vs Completed Cases overview  
- Monthly TAT trend analysis  
- SLA compliance (**Within SLA vs Breach**)  
- Executive-wise performance comparison  
- Service-wise breach distribution  

### ⏳ Pending Cases

- Total pending workload  
- Aging analysis (days elapsed)  
- Pending TAT bucket classification  

- Work status breakdown:
  - Under Process  
  - On Hold  
  - Cancelled  

- Service-wise pending case load

  ## ⚙️ Data Processing (Power Query)

- Cleaned raw Excel data by removing null/invalid records and replacing placeholder values (like `0`) with proper blanks  
- Standardized text fields using **Trim + Uppercase** to ensure consistency across reports  
- Converted key columns into correct data types (especially date fields for accurate calculations)  

- Created core metrics:
  - **TAT Days** = Completion Date − Received Date  
  - **Achieved Days** = Completion Date − Start Date  

- Standardized the **Turn Around Time** column (e.g., converting `3-5 DAYS`, `7 TO 10 DAYS` into a consistent format)

- Extracted SLA values from text:
  - **MIN SLA** and **MAX SLA** derived from TAT ranges  
  - Enabled accurate SLA comparison and breach detection  

- Final dataset was cleaned, structured, and optimized for dashboard reporting and performance analysis

  ## 🧩 Features

- Interactive filters (Year, Month, Executive, Service)  
- SLA breach detection  
- Dynamic KPI cards  
- Dual dashboard views (**Completed vs Pending**)  
- Clean and structured data model
  
## 🚀 How to Use

1. Open the `.pbix` file in Power BI Desktop  
2. Update the file path if required  
3. Refresh the data  
4. Use filters to explore insights  
