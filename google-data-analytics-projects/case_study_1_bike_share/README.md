# 🚴‍♀️ Case Study 1: Cyclistic Bike-Share Analysis

### 📘 Overview
This project is part of the **Google Data Analytics Professional Certificate**.  
The goal was to analyze Cyclistic’s bike-share data to understand how casual riders and annual members use bikes differently.

---

### 🧩 Tools Used
- Google Sheets
- R
- Tableau 

---

### 🔍 Steps in the Analysis
1. **Ask:** What is the business problem?
   - Understand how annual members and casual riders use Cyclistic bikes differently in order to design marketing strategies aimed at converting casual riders into annual members.
   
2. **Prepare:** 
   - Source: Divvy bike data (public datasets from [divvy-tripdata](https://divvy-tripdata.s3.amazonaws.com/index.html))
   - The dataset consists of 12 monthly CSV files (July 2023 – June 2024) containing 5,818,521 rides from Cyclistic’s historical trip data, made available by Motivate International Inc. under public license. Data is stored locally in  "case_study_1_bike_share/data” containing original CSVs and cleaned versions. The data follows the ROCCC framework and contains no personally identifiable information.
   - ROCCC check:
      + Reliable – First-party data from Cyclistic
      + Original – Directly from bike sensors
      + Comprehensive – Contains all needed fields
      + Current – Last 12 months (Jul 2023–Jun 2024)
      + Cited – Motivate International Inc., licensed for public use
   - Cleaned and combined 12 months of CSV files.

4. **Process:** 
   - Removed missing values and outliers.
   - Added new calculated columns (ride_length, day_of_week, etc.).

5. **Analyze:** 
   - Compared average ride duration and frequency between user types.
   - Identified peak usage times and popular stations.

6. **Share:** 
   - Created visualizations using Tableau/Matplotlib.

7. **Act:** 
   - Suggested targeted marketing strategies to increase memberships.

---

### 📊 Key Findings
- Annual members take shorter, more frequent rides.
- Casual users ride longer on weekends.
- Converting weekend casuals with discounts could increase memberships.

---

### 🖼️ Visuals
![Ride Duration Chart](visuals/ride_duration_chart.png)

---

### 💡 Learnings
This case study strengthened my skills in:
- Cleaning large datasets
- Using Google Sheets and R for descriptive analysis
- Building visuals using Tableau to communicate insights

---

### 📁 Repository Structure
data/ → Raw and cleaned datasets
analysis/ → R/Python scripts and queries
visuals/ → Charts and dashboards
README.md → Project summary (this file)
