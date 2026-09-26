# Node 1 – Flood Monitoring Firmware

## Overview

Firmware for the ESP32-S3 microcontroller running on the Flood Monitoring Node.

## Features

- Water level reading via dual HC-SR04 ultrasonic sensors
- Rainfall detection and intensity measurement
- Temperature and relative humidity monitoring via DHT11
- Local multi-sensor fusion and flood risk evaluation
- GPS coordinates acquisition and RTC timestamping
- SD card local data logging
- LoRa packet serialization and transmission to gateway

## Build & Flash

Designed for ESP-IDF or Arduino-ESP32 framework on PlatformIO / Arduino IDE.
