# System Architecture

## High-Level Architecture

```text
                ENVIRONMENT
                     |
        +------------+------------+
        |            |            |
        v            v            v
     FLOOD         FIRE/AIR    LANDSLIDE
      NODE           NODE        NODE
        |             |            |
        +-------------+------------+
                      |
                  ESP32-S3
                      |
             Multi-Sensor Fusion
                      |
               Edge Processing
                      |
                Risk Analysis
                      |
          +-----------+-----------+
          |           |           |
         GPS         RTC          SD
          |           |           |
          +-----------+-----------+
                      |
                     LoRa
                      |
                   Gateway
                      |
                  Internet
                      |
                Backend/Cloud
                  /        \
                 /          \
                v            v
          Mobile App     Web Dashboard
```

## Node-to-Gateway Flow

```text
Sensor
  ↓
ESP32-S3
  ↓
Local Processing
  ↓
Risk Level
  ↓
GPS + RTC + SD
  ↓
LoRa
  ↓
Gateway
```

## Risk Levels

Normal → Warning → High Risk → Danger
