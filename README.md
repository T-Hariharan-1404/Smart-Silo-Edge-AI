
#  Smart Silo Monitoring and Decision Support System

An IoT-based Smart Silo Monitoring and Decision Support System developed using ESP32 to monitor grain storage conditions in real time and provide intelligent recommendations for stock management. The system continuously tracks environmental parameters inside the silo, predicts spoilage risks, estimates market demand, and assists farmers in making informed decisions regarding grain storage and selling.

---


##  Introduction

Post-harvest losses due to improper storage conditions significantly affect agricultural productivity. Traditional grain storage methods lack continuous monitoring and decision-making capabilities.

This project addresses these challenges by integrating multiple sensors with an ESP32 microcontroller to create a smart grain storage ecosystem. The system monitors silo conditions, detects potential spoilage, provides security monitoring, and generates actionable recommendations for farmers.

---

##  Features

- Real-time grain level monitoring

- Temperature and humidity monitoring

- Harmful gas detection for spoilage prediction

- Light intensity measurement

- Motion detection for security

- Demand score estimation

- Rain probability prediction

- Intelligent stock selling recommendations

- Automatic gate status monitoring

- Continuous environmental surveillance

---

##  System Architecture

```text
                    +----------------+
                    |     ESP32      |
                    +--------+-------+
                             |
        ------------------------------------------------
        |          |           |          |            |
        |          |           |          |            |
   Ultrasonic    DHT11      MQ Gas      LDR      IR Sensor
      Sensor      Sensor     Sensor     Sensor
        |          |           |          |            |
        ------------------------------------------------
                             |
                             |
                   Decision Support Engine
                             |
          -------------------------------------
          |                  |                |
          |                  |                |
     Spoilage Status   Demand Analysis   Gate Control
                             |
                             |
                     Smart Silo Report
```

---

##  Hardware Components

| Component | Quantity |
|-----------|----------|
| ESP32 Development Board | 1 |
| HC-SR04 Ultrasonic Sensor | 1 |
| DHT11/DHT22 Sensor | 1 |
| MQ Gas Sensor | 1 |
| LDR Sensor | 1 |
| IR Motion Sensor | 1 |
| Servo Motor | 1 |
| Breadboard | 1 |
| Jumper Wires | As required |
| Power Supply | 1 |

---

##  Software Requirements

- Arduino IDE
- ESP32 Board Package
- C/C++ Programming Language

### Required Libraries

```cpp
#include <WiFi.h>
#include <DHT.h>
#include <ESP32Servo.h>
```


##  Pin Configuration

| Device | ESP32 Pin |
|---------|------------|
| Ultrasonic Trigger | GPIO 5 |
| Ultrasonic Echo | GPIO 18 |
| DHT Sensor | GPIO 4 |
| MQ Gas Sensor | GPIO 34 |
| LDR Sensor | GPIO 35 |
| IR Sensor | GPIO 26 |
| Servo Motor | GPIO 25 |


---

## Working Principle

### 1. Grain Level Monitoring

The ultrasonic sensor measures the distance between the sensor and grain surface. The system calculates the grain level inside the silo.

### 2. Temperature and Humidity Monitoring

The DHT sensor continuously monitors environmental conditions to ensure safe grain storage.

### 3. Gas Concentration Monitoring

The MQ gas sensor detects harmful gases produced due to grain deterioration or spoilage.

### 4. Light Intensity Monitoring

The LDR sensor measures ambient light levels within the storage environment.

### 5. Motion Detection

The IR sensor detects unauthorized movement near the storage area, enhancing security.

### 6. Intelligent Decision Support

Based on collected sensor data, the system:

- Calculates market demand score.
- Predicts rain probability.
- Determines spoilage status.
- Generates stock-selling recommendations.

---

##  Decision Support Logic

### Spoilage Detection

```text
IF Gas Concentration > Threshold
       ↓
Spoilage Risk = HIGH
ELSE
Spoilage Risk = LOW
```

### Market Recommendation

```text
IF Demand Score > 70
      → SELL STOCK

IF Demand Score between 40 and 70
      → HOLD STOCK

IF Demand Score < 40
      → DO NOT SELL STOCK
```

### Security Logic

```text
IF Motion Detected
      → Gate Opens / Alert Triggered
ELSE
      → Gate Remains Closed
```

---


##  Applications

- Smart Grain Storage
- Precision Agriculture
- Warehouse Automation
- Agricultural Supply Chain Monitoring
- Post-Harvest Loss Reduction
- Farm Inventory Management

---

##  Future Enhancements

- IoT Cloud Dashboard Integration
- Mobile Application Development
- SMS and Email Alerts
- Machine Learning-Based Demand Forecasting
- Web Dashboard for Remote Monitoring
- Automatic Ventilation Control
- GPS-Based Warehouse Tracking

---

