# Node 2 – Forest Fire & Air Quality

## Controller

ESP32-S3

## Sensors

- MQ-2
- MQ-135
- Flame Sensor
- DHT11

## Communication

- LoRa

## Supporting Modules

- GPS
- RTC
- MicroSD

## Purpose

The node monitors environmental parameters related to forest fire and
air-quality events.

## Processing

```text
Temperature
Humidity
Smoke
Gas
Flame
      ↓
ESP32-S3
      ↓
Multi-Sensor Analysis
      ↓
Fire / Air Quality Risk
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
