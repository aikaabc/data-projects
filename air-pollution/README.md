# AirQualityXplore: Identifying Pollution Patterns for Health & Policy

## Overview

AirQualityXplore investigates real-time air quality data across the United States to uncover geographic and environmental pollution patterns. The project analyzes data from the AirNow system (run by US EPA, NOAA, NPS, etc.), focusing on key metrics such as elevation, ozone (O₃), PM10, and PM2.5. The results are meant to inform health interventions and policy strategies.

Team: Aikokul Abdivalieva • Sharon Wanyana • Mathias Ndungu • Angela Ngano • Benson Osei Tutu

---

## Table of Contents

- [Project Motivation](#project-motivation)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [How to Run](#how-to-run)
- [Key Findings](#key-findings)
- [Results & Visualizations](#results--visualizations)
- [Future Work](#future-work)
- [References](#references)
- [License](#license)

---

## Project Motivation

Air pollution affects millions of people and leads to major health risks and policy challenges. Our goal is to:
- Identify regional pollution hotspots, particularly where sensitive groups are at risk.
- Explore how topography (elevation) impacts pollutant concentrations.
- Derive actionable insights to guide policymakers and public health officials.

To achieve this, we analyzed recent national monitoring data, evaluating both univariate and bivariate trends for pollutants and environmental features.

---

## 🗂️ Dataset

- **Source:** AirNow Air Quality Monitoring Data (Current)
- **Accessed:** March 4, 2025
- **Link:** [AirNow Catalog](https://nationaldataplatform.org/catalog/dataset/airnow-air-quality-monitoring-data-current)
- **Scope:** 4,940 records, 40 variables, collected worldwide on August 18, 2023
- **Attributes:** Includes monitoring site details (location, elevation), AQI for ozone, PM10, PM2.5, and other pollutants

*Complies with AirNow data usage policy.*

---

## Project Structure


---

## ⚙️ Methods & Analysis

- **Data Cleaning:** Imputed missing states for 11 sites. Standardized AQI categories per EPA guidelines.
- **EDA:** Performed univariate and bivariate analyses of elevation, ozone, PM10, and PM2.5 across 1,977 monitoring sites.
- **Visualization:** Created summary tables and plots highlighting state-by-state differences and outlier patterns.
- **Tools:** R, Excel, Tableau

---

## 🔑 Key Findings

- **Monitoring Coverage:** Highest concentration of sites in California (244) and Texas (208); lowest in DC (6) and Vermont.
- **Elevation:** Range from -2 to 3,050 meters, with outlier sites in both extremely low and high-altitude areas.
- **Ozone (O₃):** Western states (Arizona, Colorado, Utah) report the highest average O₃ AQI, potentially due to elevation and sunlight effects.
- **PM2.5:** Most states show “Good” AQI levels, reflecting successful air quality controls.
- **Variability:** Greater AQI variability in states with mixed topography (CA, AZ, TX); notable outliers suggest localized concerns.

| Measure            | Elevation | OZONE_AQI | PM10_AQI | PM2.5_AQI |
|--------------------|-----------|-----------|----------|-----------|
| Mean               | 244       | 26        | 22       | 34        |
| Median             | 3         | 25        | 18       | 28        |
| Std Dev            | 485       | 12        | 16       | 31        |
| Range              | 3052      | 77        | 195      | 454       |
| Minimum            | -2        | 0         | 0        | 0         |
| Maximum            | 3050      | 77        | 195      | 454       |
| Count              | 2017      | 1157      | 377      | 1022      |

> *See full analysis and details in [`EDA_GL-feedback.docx`](./EDA_GL-feedback.docx).*

---

## 📊 Visualizations

- State-by-state AQI summaries
- Boxplots showing distribution and outliers of AQI by elevation
- Bar charts for monitoring site counts and pollutant averages

(Visuals available in `results/visualizations/`.)

---

## 📝 Recommendations & Next Steps

- **Policy:** Focus ozone-reduction strategies in high-altitude Western states; maintain PM2.5 controls nationwide.
- **Analysis Extension:** Integrate multiyear data; link with health/emissions data for deeper insights.
- **Tool Development:** Build real-time dashboards to monitor AQI and flag regional anomalies.

---

## 📄 References

1. AirNow Air Quality Monitoring Data (Current), 2025.
2. US EPA, NOAA, NPS, state/local agencies.

---

*This project is for educational and public health analytics purposes. Data use complies with AirNow data-sharing guidelines.*
