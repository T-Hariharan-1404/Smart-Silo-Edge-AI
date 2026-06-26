# Arduino Code

This directory contains the firmware for the ESP32 microcontroller responsible for sensor data acquisition, actuator control, and communication with the dashboard.

## Responsibilities

- Read environmental sensor data
- Measure grain level
- Detect harmful gas concentration
- Monitor IR sensor status
- Control the servo-operated silo gate
- Send real-time data to the dashboard

## Hardware Interfaces

- ESP32
- DHT11 Temperature & Humidity Sensor
- HC-SR04 Ultrasonic Sensor
- MQ135 Gas Sensor
- IR Sensor
- Servo Motor


# Machine Learning Models


## Models Included

### Rain Prediction

A Random Forest Classification model predicts the likelihood of rainfall based on environmental conditions.

**Input Features**

- Temperature
- Humidity
- Historical weather parameters

**Output**

- Rain
- No Rain

---

### Demand Forecasting

A Random Forest Regression model estimates future grain demand to support intelligent buffer stock planning.

**Input Features**

- Historical demand
- Market trends
- Rain prediction

**Output**

- Predicted demand

---

## Edge AI

The trained models are optimized for deployment on embedded hardware using TinyML techniques, enabling low-latency inference without continuous cloud connectivity.
