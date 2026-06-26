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
