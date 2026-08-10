# AirWatch – Air Quality Monitoring System

AirWatch is a real-time air quality monitoring system built as a student IoT project to understand how environmental data can be collected from physical sensors, sent to the cloud, and presented in a way that is easy to understand.

The project combines an ESP32-based sensor setup with Firebase and a web dashboard. We also added a map-based view to compare our local readings with air-quality information available from external monitoring stations.

This project was developed as a hands-on exploration of IoT, sensor integration, cloud data handling, and real-time visualization.

---

## What does the project do?

The basic idea is simple:

**Sense → Send → Store → Visualize**

Environmental sensors connected to an ESP32 collect readings such as temperature, humidity, and pollution-related measurements. The ESP32 connects to Wi-Fi and sends the data to Firebase Realtime Database.

The web application then uses this data to display the current readings through a dashboard.

We also integrated a Bangalore air-quality map using the WAQI network so that the local sensor reading could be viewed alongside readings from other locations.

---

## System Flow

```text
Environmental Sensors
        ↓
      ESP32
        ↓
      Wi-Fi
        ↓
Firebase Realtime Database
        ↓
   Web Dashboard
        ↓
AQI / Sensor Visualization
        ↓
Bangalore AQI Map
