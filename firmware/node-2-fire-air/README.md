# Node 2 – Forest Fire & Air Quality Monitoring Firmware

## Overview

Firmware for the ESP32-S3 microcontroller running on the Forest Fire & Air Quality Monitoring Node.

## Features

- Smoke and flammable gas detection via MQ-2
- Air quality / hazardous gas monitoring via MQ-135
- Flame detection
- Ambient temperature and relative humidity tracking via DHT11
- Edge parameter fusion for early fire risk index calculation
- GPS coordinates acquisition and RTC timestamping
- SD card local data logging
- LoRa packet serialization and transmission to gateway

## Build & Flash

Designed for ESP-IDF or Arduino-ESP32 framework on PlatformIO / Arduino IDE.
