# AI-Powered Interconnected Environmental Monitoring & Early-Warning System

## Smart India Hackathon 2026

**Problem Statement ID:** SIH26178  
**Theme:** Disaster Management  
**PS Category:** Hardware  
**Team ID:** 169699  
**Team Name:** Apex Innovators'26

---

## 🚨 Project Overview

Our project is an AI-powered interconnected environmental monitoring
and early-warning system designed to detect multiple environmental
hazards using distributed intelligent sensor nodes.

The system consists of three specialized monitoring nodes:

- 🌊 Node 1 – Flood Monitoring
- 🔥 Node 2 – Forest Fire & Air Quality Monitoring
- ⛰️ Node 3 – Landslide Monitoring

Each node uses an ESP32-S3 as the main controller and edge-processing
unit.

The nodes collect multiple environmental parameters, perform local
processing and risk analysis, and communicate important information
through LoRa.

The processed information is forwarded through a gateway to the
backend/cloud platform and displayed through a mobile application and
web dashboard.

---

# 🎯 Problem Statement

A resilient, AI-powered environmental monitoring network that provides
early detection, localized intelligence, and actionable alerts for
floods, forest fires, pollution events, and other environmental hazards
common in India, enabling authorities and communities to shift from
reactive disaster response to proactive risk prevention.

---

# 💡 Proposed Solution

The proposed system uses multiple intelligent environmental monitoring
nodes instead of depending on a single sensor or isolated monitoring
device.

Each node:

1. Collects environmental data.
2. Performs sensor validation.
3. Combines multiple sensor parameters.
4. Performs local edge processing.
5. Determines the environmental risk level.
6. Obtains location using GPS.
7. Records time using RTC.
8. Stores important information on an SD card.
9. Communicates through LoRa.
10. Sends alerts and summaries to the central platform.

---

# 🏗️ System Architecture

```text
                    ENVIRONMENT
                         │
        ┌────────────────┼────────────────┐
        │                │                │
        ▼                ▼                ▼
   🌊 FLOOD         🔥 FIRE/AIR      ⛰️ LANDSLIDE
      NODE              NODE              NODE
        │                │                │
        └────────────────┼────────────────┘
                         │
                    ESP32-S3
                         │
             Multi-Sensor Data Fusion
                         │
                    Edge Processing
                         │
                 Risk Classification
                         │
          ┌──────────────┼──────────────┐
          │              │              │
         GPS            RTC             SD
        WHERE           WHEN           STORE
          │              │              │
          └──────────────┼──────────────┘
                         │
                        LoRa
                         │
                      Gateway
                         │
                      Internet
                         │
                  Cloud / Backend
                    │          │
                    ▼          ▼
               Mobile App   Web Dashboard
```

---

# 🌊 Node 1 – Flood Monitoring

### Sensors

* 2 × HC-SR04 Ultrasonic Sensors
* Rain Sensor
* DHT11 Temperature & Humidity Sensor

### Controller

* ESP32-S3

### Supporting Modules

* GPS
* RTC
* MicroSD
* LoRa

### Monitoring Parameters

* Water level
* Rainfall
* Temperature
* Humidity

### Risk Concept

Multiple parameters are evaluated together instead of relying on a
single sensor reading.

Example:

```text
Water Level ↑
     +
Rainfall ↑
     +
Rapid Change
     ↓
Flood Risk
```

---

# 🔥 Node 2 – Forest Fire & Air Quality

### Sensors

* MQ-2
* MQ-135
* Flame Sensor
* DHT11

### Controller

* ESP32-S3

### Supporting Modules

* GPS
* RTC
* MicroSD
* LoRa

### Monitoring Parameters

* Smoke
* Gas concentration
* Temperature
* Humidity
* Flame indication
* Air-quality related changes

### Risk Concept

```text
Temperature ↑
     +
Humidity ↓
     +
Smoke ↑
     +
Gas Change
     ↓
Fire / Air Quality Risk
```

---

# ⛰️ Node 3 – Landslide Monitoring

### Sensors

* Capacitive Soil Moisture Sensor
* MPU6050
* SW-420 Vibration Sensor
* Rain Sensor
* DHT11

### Controller

* ESP32-S3

### Supporting Modules

* GPS
* RTC
* MicroSD
* LoRa

### Monitoring Parameters

* Soil moisture
* Ground movement / tilt
* Vibration
* Rainfall
* Temperature
* Humidity

### Risk Concept

```text
Soil Moisture ↑
       +
Rainfall ↑
       +
Ground Movement
       +
Vibration
       ↓
Landslide Risk
```

---

# 🤖 Edge Intelligence

The ESP32-S3 performs local processing of sensor information.

The system is designed around multi-sensor parameter fusion rather than
making decisions from one sensor alone.

### Risk Levels

```text
🟢 NORMAL
      ↓
🟡 WARNING
      ↓
🟠 HIGH RISK
      ↓
🔴 DANGER
```

Local processing allows the node to continue monitoring even when
continuous Internet connectivity is unavailable.

---

# 📍 GPS

GPS provides the geographical location associated with each monitoring
node and environmental event.

```text
GPS
 ↓
Latitude
Longitude
 ↓
Event Location
```

---

# ⏱️ RTC

The RTC module provides reliable timestamps for sensor measurements and
alerts.

```text
Sensor Event
     ↓
RTC Timestamp
     ↓
Historical Record
```

---

# 💾 SD Card

The SD card provides local storage for:

* Sensor readings
* Risk events
* Alerts
* Timestamps
* Node information
* Important historical data

This provides local data availability during Internet interruptions.

---

# 📡 LoRa Communication

LoRa is used for long-range, low-power communication between the
distributed monitoring system and the gateway.

The system transmits compact information such as:

* Node ID
* Hazard type
* Risk level
* Sensor summary
* GPS location
* Timestamp
* Alert information

---

# 🌐 Gateway & Cloud

The gateway receives LoRa messages from the monitoring nodes.

The gateway forwards the processed information through an Internet
connection to the backend/cloud platform.

```text
Node
 ↓
LoRa
 ↓
Gateway
 ↓
Internet
 ↓
Backend / Cloud
```

---

# 📱 Mobile Application

The mobile application is intended to provide:

* Live node status
* Risk notifications
* Hazard type
* Event location
* Event time
* Sensor summaries
* Historical information
* Alerts

---

# 💻 Web Dashboard

The web dashboard is intended for centralized monitoring.

It can display:

* Node locations
* Current sensor values
* Risk levels
* Active alerts
* Historical data
* Node health
* Environmental trends

---

# 🔄 Complete Data Flow

```text
Environmental Sensors
        ↓
Sensor Data Collection
        ↓
ESP32-S3
        ↓
Multi-Sensor Fusion
        ↓
Edge Processing / AI
        ↓
Risk Classification
        ↓
GPS + RTC + SD
        ↓
LoRa Communication
        ↓
Gateway
        ↓
Internet
        ↓
Cloud / Backend
        ↓
 ┌───────────────┐
 │               │
 ▼               ▼
Mobile App   Web Dashboard
```

---

# ✨ Innovation & Uniqueness

* Multi-hazard environmental monitoring
* Three specialized intelligent nodes
* Multi-sensor parameter fusion
* Local edge processing
* GPS-based event location
* RTC-based event timestamping
* SD-card local storage
* Long-range LoRa communication
* Mobile application
* Web dashboard
* Modular and scalable architecture

---

# 📊 Risk Classification

| Risk Level   | Meaning                                            |
| ------------ | -------------------------------------------------- |
| 🟢 Normal    | Environmental parameters are within expected range |
| 🟡 Warning   | Early abnormal condition detected                  |
| 🟠 High Risk | Significant hazard indicators detected             |
| 🔴 Danger    | Immediate or severe risk condition detected        |

---

# 🔧 Hardware

Main hardware components:

* ESP32-S3
* HC-SR04
* Rain Sensor
* DHT11
* MQ-2
* MQ-135
* Flame Sensor
* Capacitive Soil Moisture Sensor
* MPU6050
* SW-420
* GPS Module
* RTC Module
* MicroSD Module
* LoRa Module
* Buzzer
* LEDs
* Solar Panel
* Battery
* Charging / Protection Circuit
* Voltage Regulation

---

# 🧠 Software

* ESP32-S3 Firmware
* Edge Processing
* Risk Classification
* LoRa Communication
* Gateway Software
* Backend APIs
* Mobile Application
* Web Dashboard

---

# 📚 Documentation

| Document            | Description                             |
| ------------------- | --------------------------------------- |
| [Problem Statement](docs/problem-statement.md)   | SIH26178 details                        |
| [System Architecture](docs/system-architecture.md) | Complete system flow                    |
| [AI Methodology](docs/ai-methodology.md)      | Edge processing and risk classification |
| [Hardware](docs/hardware.md)            | Components and connections              |
| [Communication](docs/communication.md)       | LoRa and gateway architecture           |
| [References](docs/references.md)          | Datasheets and research papers          |

---

# 👥 Team

## Apex Innovators'26

**Team ID:** 169699

---

# 🏆 Smart India Hackathon 2026

**SIH Problem Statement:** SIH26178  
**Theme:** Disaster Management  
**Category:** Hardware  

---

## Sense • Analyze • Connect • Alert
