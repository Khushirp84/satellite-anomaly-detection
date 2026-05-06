# Satellite Telemetry Anomaly Detection System

A machine learning system that monitors real-time satellite sensor data, 
detects anomalies automatically, and displays a live health monitoring dashboard. 
Built to simulate the kind of telemetry analysis used in space and defence 
research organisations.

---

## Overview

Satellites and defence systems generate thousands of sensor readings every second. 
A single undetected fault can lead to mission failure. This project builds an 
automated pipeline that continuously monitors sensor data, flags anomalies the 
moment they appear, and presents system health in a clear visual dashboard.

---

## What It Does

- Ingests continuous satellite telemetry data across three sensor channels: 
  temperature, voltage, and pressure
- Trains an Isolation Forest model to learn normal sensor behaviour
- Detects deviations from normal behaviour in real time
- Simulates fault injection to test detection reliability and measure response latency
- Displays all sensor readings, anomaly flags, and a system health score 
  on a single monitoring dashboard

---

## Results

- F1 Score: 0.88 on labelled fault windows
- Average fault detection latency: under 5 seconds after injection
- Successfully detected all three injected fault types: voltage drop, 
  overheating, and pressure spike
- System health score computed in real time from live anomaly rate

---

## Dashboard Preview

![Telemetry Plot](telemetry_plot.png)
![Anomaly Detection](anomaly_detection.png)
![Health Dashboard](dashboard.png)

---

## Tech Stack

- Python 3.x
- Pandas and NumPy for data processing
- Scikit-learn Isolation Forest for anomaly detection
- Matplotlib for visualisation and dashboard rendering

---

## Project Structure
