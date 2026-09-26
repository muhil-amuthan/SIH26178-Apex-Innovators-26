# Hardware Documentation

## Common Hardware

Each monitoring node is based on:

- ESP32-S3
- GPS
- RTC
- MicroSD
- LoRa
- Power supply
- Solar / battery system

---

# Node 1 – Flood

| Component | Purpose |
|---|---|
| ESP32-S3 | Controller and edge processing |
| HC-SR04 ×2 | Water-level measurement |
| Rain Sensor | Rainfall indication |
| DHT11 | Temperature and humidity |
| GPS | Location |
| RTC | Timestamp |
| MicroSD | Local storage |
| LoRa | Long-range communication |

---

# Node 2 – Fire / Air

| Component | Purpose |
|---|---|
| ESP32-S3 | Controller and edge processing |
| MQ-2 | Smoke / gas indication |
| MQ-135 | Air-quality related sensing |
| Flame Sensor | Flame detection |
| DHT11 | Temperature and humidity |
| GPS | Location |
| RTC | Timestamp |
| MicroSD | Local storage |
| LoRa | Long-range communication |

---

# Node 3 – Landslide

| Component | Purpose |
|---|---|
| ESP32-S3 | Controller and edge processing |
| Soil Moisture | Soil condition |
| MPU6050 | Motion / tilt |
| SW-420 | Vibration |
| Rain Sensor | Rainfall |
| DHT11 | Temperature and humidity |
| GPS | Location |
| RTC | Timestamp |
| MicroSD | Local storage |
| LoRa | Long-range communication |

---

# Power

The intended system can use:

Solar Panel
     ↓
Charging / Protection
     ↓
Battery
     ↓
Voltage Regulation
     ↓
ESP32-S3 + Sensors
