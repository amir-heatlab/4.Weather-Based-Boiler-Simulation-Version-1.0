# Smart Boiler Thermal Simulation & Predictive Maintenance System

## Overview

This project presents a physics-informed thermal simulation of a residential heating system using real-world meteorological data. The goal is to model boiler behavior under varying environmental conditions and generate a machine learning-ready dataset for predictive maintenance and failure risk analysis.

The system integrates real climate data with engineered thermal features to simulate heating demand, system load, and operational stress on residential boilers.

---

## Problem Statement

Residential boilers operate under varying environmental conditions that directly affect efficiency and failure risk. However, most systems lack predictive intelligence.

This project addresses the question:

Can boiler stress and potential failure risk be predicted using only environmental temperature data and engineered thermal behavior models?

---

## Data Source

- Historical weather data from Open-Meteo API  
- Location: Kermanshah, Iran  
- Time range: October 2024 – March 2025  
- Features:
  - Maximum air temperature at 2 meters
  - Minimum air temperature at 2 meters
  - Mean air temperature at 2 meters

---

## Feature Engineering

### 1. Warm-up Time
Estimated time required for the heating system to reach target temperature based on external conditions.

### 2. Radiator Water Temperature
Physics-informed estimation of supply water temperature based on outdoor temperature.

### 3. Risk Label
Rule-based classification of operational stress:

- Low Risk
- High Risk

---

## Methodology

1. Collect real-world weather data via API  
2. Preprocess time-series dataset  
3. Simulate thermal behavior of heating system  
4. Engineer features (Warm-up Time, Radiator Temperature)  
5. Define risk labels using threshold-based rules  
6. Perform exploratory data analysis and visualization  

---

## Technologies

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Requests  
- Jupyter Notebook  

---

## Project Structure

Boiler-Thermal-Simulation/
├── boiler_thermal_simulation.ipynb
├── boiler_dataset.csv
├── main.py
└── README.md

---

## Key Insights

- Heating demand is strongly dependent on outdoor temperature  
- Warm-up time increases significantly in colder conditions  
- Radiator supply temperature follows adaptive nonlinear behavior  
- Rule-based thermal modeling can approximate system stress patterns  

---

## Future Work

- Integration of real boiler sensor data (pressure, flow rate, gas consumption)  
- Hybrid physics + machine learning modeling  
- Predictive maintenance using Decision Tree, Random Forest, XGBoost  
- Real-time monitoring dashboard  
- Digital Twin architecture for HVAC systems  

---

## Research Potential

This project can be extended into:

- Predictive Maintenance Systems  
- Smart HVAC Optimization  
- Energy Efficiency Modeling  
- Digital Twin Simulation Systems  

---

## Author

Independent research project in applied machine learning and thermal system modeling.

---

## License

Educational and research purposes only.
