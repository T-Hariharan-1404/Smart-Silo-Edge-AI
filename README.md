# Smart-Silo-Edge-AI


An IoT and Edge AI-based grain storage system designed to reduce post-harvest losses and improve buffer stock management. The system continuously monitors grain storage conditions and uses TinyML-powered Random Forest models to predict rainfall and market demand, enabling smarter decisions and automated protection.

---

##  About the Project

Traditional grain storage systems are mostly reactive, meaning problems are addressed only after they occur. Factors such as humidity, temperature, gas formation, and changing market demand can lead to spoilage and financial losses.

Smart Silo Edge AI aims to solve these challenges by combining IoT sensors with machine learning to create an intelligent and affordable storage solution.

The system monitors storage conditions in real time, predicts rainfall and demand trends, and automatically controls a protective gate to help maintain grain quality and optimize inventory planning.

---

##  Features

- Real-time monitoring of temperature and humidity
- Grain level measurement using ultrasonic sensing
- Gas detection for spoilage prevention
- Rain prediction using a Random Forest model
- Demand forecasting for intelligent buffer stock management
- Automatic gate control using a servo motor
- Dashboard for visualization and alerts
- Low-cost and scalable design suitable for rural deployment

---

##  Hardware Used

- ESP32 Microcontroller
- DHT11 Sensor
- Ultrasonic Sensor
- MQ135 Gas Sensor
- IR Sensor
- Servo Motor

---

##  Software and Tools

- Python
- Flask
- Streamlit
- Pandas
- Scikit-Learn
- TinyML
- Random Forest Machine Learning Models

---

##  Machine Learning Models

### Rain Prediction

A Random Forest classification model is used to predict whether rainfall is likely to occur based on environmental conditions.

**Inputs**
- Temperature
- Humidity
- Historical weather data

**Output**
- Rain / No Rain

### Demand Forecasting

A Random Forest regression model is used to estimate future grain demand.

**Inputs**
- Historical demand data
- Pricing data
- Rain prediction

**Output**
- Predicted demand levels

---

##  System Workflow

```text
Sensors
   ↓
ESP32 Data Collection
   ↓
Machine Learning Prediction
   ↓
Risk Analysis
   ↓
Dashboard and Alerts
   ↓
Automated Gate Control
```

---

##  Applications

- Government food warehouses
- FCI storage centers
- Agricultural cooperatives
- Rural grain storage facilities
- Supply chain and logistics hubs

---

##  Contribution to Sustainable Development Goals

- **SDG 2 – Zero Hunger**
  - Reduces grain losses and improves food security.

- **SDG 9 – Industry, Innovation and Infrastructure**
  - Promotes smart agricultural infrastructure.

- **SDG 12 – Responsible Consumption and Production**
  - Minimizes wastage through data-driven decisions.

- **SDG 13 – Climate Action**
  - Supports weather-aware storage planning.

---

##  Future Enhancements

- AI-based spoilage prediction
- SMS alerts for farmers
- Multi-silo network optimization
- Cloud integration and advanced analytics
- Integration with government procurement systems

---


##  Hackathon

**ElectroHack 2.0**

---
