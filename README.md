# Smart Home Occupancy Detection Using Machine Learning

A machine-learning-based occupancy detection system that uses environmental sensor measurements to classify whether an indoor environment is **occupied or unoccupied**.

This project is part of the research study:

> **Smart Home Devices: Applications, Benefits, and Challenges**

The implementation focuses on the practical problem of **occupancy detection using environmental IoT sensor data** and compares three supervised machine-learning models:

- Logistic Regression
- Random Forest
- XGBoost

---

## 📌 Project Overview

Smart-home systems require reliable information about whether an indoor environment is occupied to support context-aware automation.

Occupancy information can be used for applications such as:

- 💡 Intelligent lighting control
- 🌡️ HVAC control
- ⚡ Energy management
- 🏠 Context-aware home automation
- 🔐 Security systems
- 📅 Occupant-aware device scheduling

Instead of relying only on fixed schedules or dedicated occupancy sensors, this project investigates whether environmental measurements such as **temperature, humidity, light, and CO₂** can be used with machine-learning models to detect occupancy.

---

## 🎯 Objectives

The main objectives of this project are:

1. Analyze environmental sensor data for occupancy detection.
2. Preprocess and prepare the dataset for machine learning.
3. Select relevant environmental features.
4. Implement three classification algorithms.
5. Evaluate the models using multiple classification metrics.
6. Compare the models using a common test dataset and evaluation protocol.
7. Analyze feature importance for tree-based models.
8. Study the feasibility of environmental-sensor-based occupancy detection for smart-home/IoT applications.

---

## 📊 Dataset

### UCI Occupancy Detection Dataset

The project uses the publicly available **UCI Occupancy Detection Dataset**.

The original dataset was collected from an **office environment** using environmental sensors. Occupancy ground truth was obtained using timestamped observations.

### Dataset Statistics

| Property | Value |
|---|---:|
| Total observations | 20,560 |
| Predictive features | 6 |
| Target variable | Occupancy |
| Task | Binary Classification |
| Missing values | 0 |
| Duplicate records | 0 |
| Occupied observations | 4,750 |
| Unoccupied observations | 15,810 |

### Features

| Feature | Description | Unit |
|---|---|---|
| `id` | Record identifier | — |
| `date` | Timestamp | Date/Time |
| `Temperature` | Environmental temperature | °C |
| `Humidity` | Relative humidity | % |
| `Light` | Light intensity | Lux |
| `CO2` | Carbon dioxide concentration | ppm |
| `HumidityRatio` | Derived humidity measure | kg water-vapor/kg air |
| `Occupancy` | Occupancy status | 0/1 |

For the primary machine-learning experiment, the following five environmental features were used:

```text
Temperature
Humidity
Light
CO2
HumidityRatio
