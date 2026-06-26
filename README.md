
# Smart Boiler Thermal Simulation & Predictive Maintenance System

## Overview

This project presents a physics-informed thermal simulation of a residential heating system using real-world meteorological data. The goal is to model boiler behavior under varying environmental conditions and generate a machine learning-ready dataset for predictive maintenance and failure risk analysis.

The system integrates real climate data with engineered thermal features to simulate heating demand, system load, and operational stress on residential boilers.

---

## Problem Statement

Residential boilers often operate under varying environmental conditions that directly affect their efficiency and failure risk. However, most systems lack predictive intelligence.

This project addresses the following question:

> Can we predict boiler stress and potential failure risk using only environmental temperature data and engineered thermal behavior models?

---

## Data Source

- Historical weather data is retrieved from the **Open-Meteo API**
- Location: Kermanshah, Iran
- Time range: October 2024 – March 2025
- Features:
  - Max Temperature (2m)
  - Min Temperature (2m)
  - Mean Temperature (2m)

---

## Feature Engineering

To simulate boiler behavior, the following engineered features were created:

### 1. Warm-up Time
Estimated time required for the heating system to reach target temperature based on external conditions.

### 2. Radiator Water Temperature
A physics-informed approximation of supply water temperature adjusted based on outdoor temperature.

### 3. Risk Label
A rule-based classification system defining operational stress levels:

- **Low Risk**
- **High Risk**

---

## Methodology

The system follows a step-by-step pipeline:

1. Data collection from real-world weather API
2. Data preprocessing and time-series formatting
3. Thermal behavior simulation using engineered rules
4. Feature creation (Warm-up Time, Radiator Temperature)
5. Risk labeling based on thermal thresholds
6. Exploratory data analysis and visualization

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Requests (API handling)
- Jupyter Notebook

---

## Project Structure

