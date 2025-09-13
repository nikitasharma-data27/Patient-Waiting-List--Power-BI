# 🏥 Patient Wait List Analysis – Power BI Dashboard

## 📌 Project Overview
This project is a **Power BI dashboard** that analyzes patient wait lists by combining Inpatient and Outpatient data, enabling stakeholders to track key metrics such as Average and Median wait lists dynamically.  
The dashboard uses **interactive slicers** and **dynamic DAX measures** to help users toggle between Average/Median views, filter by Case Type, Specialty, and visualize trends effectively.

---

## 🎯 Key Features
- **Data Modeling**: Combined Inpatient & Outpatient data into a single `All_Data` table using Power Query.
- **Specialty Mapping**: Used a separate mapping file to group specialties into meaningful buckets.
- **Dynamic Slicers**: 
  - Case Type  
  - Special Name  
  - Average/Median Toggle  
- **Dynamic Titles**: Auto-updating chart headers based on user selection.
- **DAX Measures**:
  - `Average Wait List` → `AVERAGE(All_Data[Total])`
  - `Median Wait List` → `MEDIAN(All_Data[Total])`
  - `Avg/Med Wait List` → Switches between Avg/Median dynamically
  - `Dynamic Title` → Displays selected calculation type
- **Visuals Used**:
  - Doughnut Chart
  - Clustered Column Chart
  - Line Chart (Trend over Time)
  - Multi-Row Card (Top 5 Categories)
  - Matrix View (Detailed Drilldown)

---

## 🛠 Tools & Technologies
- **Power BI Desktop**
- **Power Query (M Language)** – Data cleaning, transformation, and appending
- **DAX (Data Analysis Expressions)** – Calculations & dynamic measures
- **Excel / CSV Files** – Specialty mapping & source data
- **Canva / PowerPoint** – Background design (optional)

---

## 📊 Dashboard Preview
<img width="1164" height="655" alt="Screenshot 2025-09-13 200231" src="https://github.com/user-attachments/assets/f084769d-dda8-4348-b489-afda98302d95" />
<img width="1312" height="732" alt="Screenshot 2025-09-13 232855" src="https://github.com/user-attachments/assets/65d3f77e-88be-4cfa-b7f3-4a3013638a8a" />


---

## 🚀 How to Use
1. Download the `.pbix` file from this repository.
2. Open it in **Power BI Desktop**.
3. Use slicers to switch between:
   - **Average** / **Median**
   - **Case Types** (Inpatient, Outpatient, Day Case)
   - **Specialty Groups**
4. Explore visuals to analyze patient wait lists by latest month, previous year, and specialty trends.

---

## 📈 Data Model
- **All_Data** – Combined table of Inpatient + Outpatient
- **Specialty Mapping** – Relationship created with `Specialty_Name`
- **Calculation Method Table** – Static table with "Average" & "Median" options for slicer control

---

## 🔄 Maintenance
This dashboard is designed for **monthly refresh** and routine maintenance using Power BI Service scheduled refresh.

---

## 📌 Author
Nikita Sharma  
💼 *Data Analyst / Power BI Developer*   
📧 nikitasharma2727nikki@gmail.com
