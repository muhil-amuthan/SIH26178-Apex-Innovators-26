# Node 1 – Flood Monitoring

## Controller

ESP32-S3

## Sensors

- HC-SR04 ×2
- Rain Sensor
- DHT11

## Communication

- LoRa

## Supporting Modules

- GPS
- RTC
- MicroSD

## Purpose

The flood node monitors water level, rainfall, temperature and humidity.

## Processing

```text
Water Level
Rainfall
Temperature
Humidity
      ↓
ESP32-S3
      ↓
Multi-Sensor Analysis
      ↓
Flood Risk
```

## Risk Levels

* Normal
* Warning
* High Risk
* Danger

## Prototype Status

Add actual prototype status here:

* [ ] Sensors tested
* [ ] ESP32-S3 tested
* [ ] LoRa tested
* [ ] GPS tested
* [ ] RTC tested
* [ ] SD storage tested
* [ ] Risk classification tested
