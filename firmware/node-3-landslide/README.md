# Node 3 – Landslide Monitoring Firmware

## Overview

Firmware for the ESP32-S3 microcontroller running on the Landslide Monitoring Node.

## Features

- Soil saturation tracking via capacitive soil moisture sensor
- Tilt, orientation, and ground acceleration via MPU6050 6-axis IMU
- Seismic / high-frequency vibration detection via SW-420
- Rainfall monitoring and temperature/humidity via DHT11
- Multi-parameter heuristic landslide risk classification
- GPS coordinates acquisition and RTC timestamping
- SD card local data logging
- LoRa packet serialization and transmission to gateway

## Build & Flash

Designed for ESP-IDF or Arduino-ESP32 framework on PlatformIO / Arduino IDE.
