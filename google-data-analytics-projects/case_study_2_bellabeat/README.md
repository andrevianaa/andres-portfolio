# ⌚ Case Study 2: Bellabeat Leaf Analysis

### 📘 Overview
This project is part of the **Google Data Analytics Professional Certificate**.  
The goal is to discover trends in smart-device usage, understand how these trends apply to Bellabeat customers.

---

### 🧩 Tools Used
- Google Sheets

---

### 🔍 Steps in the Analysis
**1. ASK PHASE (Deliverable: Clear Business Task)**

Business Task: As a junior data analyst on the Bellabeat marketing analytics team, I have been asked to analyze smart-device usage data to gain insight into how consumers use non-Bellabeat smart devices. The goal is to discover trends in smart-device usage, understand how these trends apply to Bellabeat customers, and provide high-level recommendations that can influence Bellabeat’s marketing strategy for the Bellabeat Leaf product.

Key stakeholders:
- Urška Sršen (CCO & co-founder)
- Sando Mur (co-founder & mathematician)
- Bellabeat marketing analytics team

Chosen Bellabeat product to focus on: Leaf (classic wellness tracker – bracelet/necklace/clip).
   
**2. PREPARE PHASE (Deliverable: Description of data sources)**

Dataset used: FitBit Fitness Tracker Data (CC0: Public Domain)
Source: https://www.kaggle.com/datasets/arashnic/fitbit
Made available by Möbius
30 eligible Fitbit users, March 12, 2016 – May 12, 2016 (31 days)

ROCCC check (you must write this):
- Reliable – Medium (small sample, self-reported via Fitbit)
- Original – High (direct from Fitbit users via Amazon Mechanical Turk)
- Comprehensive – Medium (covers steps, calories, intensity, heart rate, sleep – but no demographics, no gender, no age)
- Current – Low (data from 2016 – outdated for 2025 trends)
- Cited – High (widely used in Google Data Analytics Certificate)

Limitations:
Only 30 users (sample size too small for statistical significance)
No demographic data (we don’t know if users are women – Bellabeat’s target)
Data is 9 years old
Only 31 days of data

The primary dataset is the FitBit Fitness Tracker Data (CC0: Public Domain) from Kaggle, containing minute-level activity, heart rate, and sleep data for 30 Fitbit users over 31 days in 2016. While the dataset is original and well-cited, it has limitations: small sample size, lack of demographic information (especially gender), and outdated data. These limitations will be acknowledged in the final recommendations.

**3. PROCESS PHASE**

In BigQuery, I created cleaned versions of the main tables by converting string dates to proper DATE types, removing NULL step values, and creating aggregated views. I classified users into activity levels based on CDC guidelines (<5000 steps = sedentary, etc.). All cleaning steps are reproducible in the SQL script above.

**4. ANALYZE PHASE**


**5. SHARE PHASE**



**6. ACT PHASE (High-level recommendations)**

Top 3 final recommendations:

- A. Target “Lightly Active” women with Leaf notifications
   + 40% of users fall into 5,000–7,500 steps. Send personalized “You’re close to 7,500 steps!” nudges via the Bellabeat app to move them into “Fairly Active.”
- B. Launch a “Reduce Sedentary Time” campaign
   + Users spend ~16.5 hours sedentary daily. Promote Leaf’s sedentary alerts and hourly movement reminders in social media ads targeting office workers.
- C. Improve sleep tracking adoption
   + Only 24/33 users logged sleep. Highlight Leaf’s superior sleep accuracy vs Fitbit in YouTube ads and create a “Sleep Better Challenge” inside the Bellabeat membership program.

### 📁 Repository Structure
data/ → Raw and cleaned datasets
analysis/ → Google Sheets analysis
visuals/ → Charts and dashboards
README.md → Project summary (this file)
