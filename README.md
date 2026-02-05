# EV Adoption and Charging Infrastructure Analysis in Washington State

![Python](https://img.shields.io/badge/Python-Data%20Analysis-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Processing-brightgreen)
![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Visualisation-purple)
![Urban Planning](https://img.shields.io/badge/Application-Urban%20Planning-success)

This project analyses the relationship between **electric vehicle (EV) adoption**, **charging infrastructure availability**, and **vehicle capability** across cities in Washington State. By integrating EV registration data, public charging station data, and EV technical specifications, the project provides an interactive, data-driven view of how EV ecosystems evolve over time.

The main output is an **animated bubble scatterplot** that visualises how cities change as adoption grows and charging infrastructure expands.

---

## Project Motivation

As EV adoption accelerates, cities must ensure that charging infrastructure keeps pace with demand. While some cities invest early in charging networks, others experience rapid EV growth without proportional infrastructure expansion, creating potential future bottlenecks.

This project aims to:
- Examine how EV adoption and charging infrastructure scale together  
- Identify cities where infrastructure may lag behind adoption  
- Explore how improvements in EV range evolve alongside infrastructure growth  

The findings are relevant for **urban planners, policymakers, and sustainability analysts** seeking evidence-based insights into EV readiness.

---

## Data Overview

The analysis combines three datasets:

- **Washington State Electric Vehicle Population Data (DOL)**  
  Over **264,000 EV registration records**, capturing adoption trends across cities and model years.

- **Alternative Fuel Stations Dataset (NREL / U.S. DOE)**  
  Public charging station locations and charger counts, used to derive **city-level charging infrastructure intensity**.

- **EV Specifications Dataset (Kaggle)**  
  Technical attributes for EV models, including **driving range and battery characteristics**, enabling analysis of vehicle capability.

Together, these datasets introduce real-world data variety across administrative, infrastructure, and technical domains.

---

## Methodology Summary

- Cleaned and standardised vehicle, geographic, and technical fields  
- Handled missing values using median and modal imputation  
- Linked EV registrations to technical specifications using standardised make-model keys  
- Aggregated charging infrastructure data to the **city level**  
- Derived an infrastructure intensity metric: **charging ports per 100 EVs**  
- Grouped results by **city and model year** to support temporal analysis  

Care was taken to preserve adoption trends and avoid data loss during integration.

---

## Visualisation Design

The final visualisation is an **interactive animated bubble scatterplot built with Plotly**, encoding multiple dimensions:

- **X-axis:** Charging ports per 100 EVs (infrastructure intensity)  
- **Y-axis:** Average EV range (vehicle capability)  
- **Bubble size:** Number of registered EVs (adoption scale)  
- **Animation:** Model year (temporal evolution)  

Hover tooltips provide detailed values on demand, while animation enables users to observe how cities evolve over time rather than relying on static comparisons.

---

## Key Insights

- Cities with stronger charging infrastructure generally support **larger EV fleets and higher-range vehicles**  
- Some cities show **EV adoption growing faster than infrastructure**, signalling future pressure on charging networks  
- Improvements in vehicle capability often coincide with infrastructure expansion, highlighting their interdependence  

---

## Technologies Used

- **Python**
- **Pandas** – data cleaning, transformation, and aggregation  
- **Plotly** – interactive and animated visualisation  

---

## Potential Extensions

- Geographic mapping of infrastructure gaps  
- Charger-type analysis (Level 2 vs DC fast charging)  
- Finer-grained temporal modelling or forecasting  
- Comparison with other U.S. states 
