# COVID-19 India Dashboard | Tableau Project

## 📌 Project Overview
This project analyzes COVID-19 trends across Indian states, including infection growth, mortality and recovery rates, vaccination progress, and state-wise testing volumes and outcomes using interactive Tableau dashboards.

The goal is to provide data-driven insights to support public health decision-making through visual analytics.

🔗 **Live Interactive Dashboard (Tableau Public):**
[View Dashboard Here](https://public.tableau.com/shared/2HYGHHQJ4?:display_count=n&:origin=viz_share_link)

---

## 🎯 Business Problem

During the COVID-19 pandemic, decision-makers faced challenges in:
- Monitoring state-wise infection trends
- Tracking vaccination progress
- Understanding mortality and recovery rates
- Allocating healthcare resources effectively

This dashboard consolidates multiple datasets to provide a unified analytical view of the pandemic in India.

---

## 📊 Dataset

Source:

🔗 **Kaggle: COVID-19 in India Dataset:**
[View Dataset Here](https://www.kaggle.com/datasets/sudalairajkumar/covid19-in-india)

🔗 **India GIS Map Dataset:**
[Required Map Dataset Here](https://simplemaps.com/gis/country/in)

Key attributes used:
- Date
- State/Union Territory
- Confirmed Cases
- Cured Cases
- Deaths
- First & Second Dose Administered
- Testing Data

---

## ⚙️ Data Preparation

Following preprocessing was performed to ensure analytical accuracy and consistency across datasets:

- Handled missing values using Tableau’s `IFNULL()` function to avoid distortion in trend calculations.
- Converted key metrics (Confirmed, Deaths, Cured, First Dose, Second Dose, Testing Counts) into appropriate numeric formats.
- Removed unrealistic or inconsistent entries to maintain data reliability.
- Created calculated fields to enhance interpretability:
  - **Mortality Rate** = Deaths / Confirmed Cases
  - **Recovery Rate** = Cured Cases / Confirmed Cases
- Performed dataset blending to integrate:
  - COVID case data
  - Vaccination data
  - Testing data
  - Geographic GIS mapping dataset

These steps ensured data integrity and enabled meaningful cross-state comparisons and time-series analysis.


## 📈 Dashboard Components

The dashboard integrates multiple visual elements to provide a comprehensive analytical view of the pandemic.

### 1️⃣ Dual-Axis Line Chart – Trend & Wave Analysis

This visualization tracks Confirmed, Cured, and Death counts over time using a dual-axis structure.

- Identifies infection waves and peak periods
- Highlights divergence between confirmed and recovered cases
- Clearly captures the significant surge during early 2021 (second wave)
- Enables filtering by state and year for localized analysis

This chart supports temporal trend analysis and outbreak monitoring.

---

### 2️⃣ Geographic Map – Regional Mortality Distribution

The India map visualizes state-wise death intensity using color gradients.

- Darker regions represent higher mortality concentration
- Supports rapid identification of high-impact states
- Integrates mortality rate and total deaths in tooltips for deeper interpretation

This visualization aids in geographic risk assessment and resource allocation planning.

---

### 3️⃣ Vaccination Progress – First vs Second Dose Comparison

A horizontal bar chart comparing first and second dose administration across states.

- Reveals gaps between initial vaccination and full vaccination
- Identifies potential drop-off patterns
- Helps assess public participation and awareness effectiveness

This provides insight into vaccination campaign efficiency.

---

### 4️⃣ Vaccine Type Distribution

Compares total doses administered by vaccine type (Covishield, Covaxin, Sputnik).

- Evaluates distribution balance
- Highlights resource allocation patterns
- Assesses dependency on specific vaccine types

Supports strategic supply chain and public health evaluation.

---

### 5️⃣ Testing Volume & Outcomes (Stacked Bar Chart)

Displays total samples tested, positive cases, and negative cases state-wise.

- Evaluates testing scale and intensity
- Assesses detection efficiency
- Examines correlation between testing expansion and confirmed case spikes

This visualization provides insight into disease detection capability and testing responsiveness.


## 🧠 Key Insights

- A significant surge in confirmed and death cases during early 2021 indicates the second pandemic wave across multiple states.
- Maharashtra shows a disproportionately high mortality concentration compared to several other regions.
- Noticeable gap between first and second dose administration suggests behavioral, logistical, or awareness challenges.
- Increased testing volumes correlate with higher detected case counts, indicating improved detection rather than purely increased spread.
- Recovery rates improved over time, potentially reflecting enhanced treatment protocols and vaccination impact.

These insights demonstrate how visual analytics can support data-driven public health decisions.


## 📷 Dashboard Preview

![Dashboard](dashboard.png)

---
## 🎓 Learning Outcomes

Through this project, I developed practical expertise in:

- Data cleaning and preprocessing within BI environments
- Creating calculated fields for performance metrics
- Designing interactive, user-friendly dashboards
- Implementing geographic visualizations using GIS data blending
- Transforming raw datasets into decision-support insights

The project strengthened my ability to translate complex datasets into intuitive, executive-level visual narratives.


