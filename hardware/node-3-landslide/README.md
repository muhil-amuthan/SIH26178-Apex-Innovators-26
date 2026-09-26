# Node 3 – Landslide Monitoring

## Controller

ESP32-S3

## Sensors

- Capacitive Soil Moisture
- MPU6050
- SW-420 Vibration
- Rain Sensor
- DHT11

## Communication

- LoRa

## Supporting Modules

- GPS
- RTC
- MicroSD

## Purpose

The node monitors soil moisture, vibration, ground movement and
rainfall-related conditions associated with landslide risk.

## Processing

```text
Soil Moisture
Ground Movement
Vibration
Rainfall
      ↓
ESP32-S3
      ↓
Multi-Sensor Analysis
      ↓
Landslide Risk
```

## Risk Levels

* Normal
* Warning
* High Risk
* Danger

## Prototype Status

* [ ] Sensors tested
* [ ] ESP32-S3 tested
* [ ] LoRa tested
* [ ] GPS tested
* [ ] RTC tested
* [ ] SD storage tested
* [ ] Risk classification tested
