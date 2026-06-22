# LiDAR-Based Predictive Road Surface Anomaly Detection and Automatic Braking System

## Overview

This project uses TF-Luna LiDAR, Raspberry Pi 4, and Machine Learning to detect potholes, bumps, and road surface anomalies in real time. The system predicts hazardous road conditions and automatically activates braking to improve vehicle safety.

## Hardware Components

- Raspberry Pi 4 Model B
- TF-Luna LiDAR Sensor
- L298N Motor Driver
- SG90 Servo Motor
- DC Gear Motors
- LM2596 Buck Converter
- Wheel Encoder
- Li-Po Battery

## Technologies Used

- Python
- LiDAR Sensing
- Time-of-Flight Measurement
- Random Forest Machine Learning
- Embedded Systems
- Raspberry Pi

## Working Principle

1. TF-Luna LiDAR continuously measures road distance.
2. Raspberry Pi processes sensor readings.
3. Features are extracted from distance data.
4. Random Forest classifies road conditions.
5. Stopping distance is calculated.
6. Automatic braking is activated when required.

---

## Block Diagram

![Block Diagram](screenshots/block_diagram.jpg)

The complete system architecture showing sensing, processing, braking, and drive control units.

---

## Time-of-Flight Measurement Principle

![Time of Flight](screenshots/time_of_flight_principle.jpg)

The TF-Luna LiDAR calculates distance using the Time-of-Flight (ToF) principle:

D = (c × T) / 2

where:
- D = Distance
- c = Speed of light
- T = Round-trip travel time

---

## Flat Surface Detection

![Flat Surface](screenshots/flat_surface_measurement.jpg)

Normal road conditions produce stable distance readings that establish the baseline reference distance.

---

## Pothole Detection

![Pothole Detection](screenshots/pothole_detection.jpg)

When the measured distance increases beyond the baseline threshold, the system detects a pothole and evaluates braking requirements.

---

## Random Forest Classifier

![Random Forest](screenshots/random_forest_classifier.jpg)

Machine Learning model trained to classify:

- Normal Road
- Bump
- Pothole

based on extracted LiDAR features.

---

## System Flowchart

![Flowchart](screenshots/flowchart.jpg)

Complete processing pipeline:

LiDAR Acquisition → Surface Analysis → Feature Extraction → Random Forest Classification → Braking Decision

---

## Distance Measurement Results

![Distance Graph](screenshots/distance_measurement_graph.jpg)

Experimental results showing measured distances for:

- Normal Surface
- Small Pothole
- Medium Pothole
- Deep Pothole

---

## Project Report

📄 [View Full Report](LiDAR_Project_Report.pdf)

## Author

Sam Benjamin R
