# Communication Architecture

## LoRa Communication

LoRa is used as the long-range, low-power communication technology
between distributed monitoring nodes and the gateway.

## Data Packet

A compact monitoring packet can contain:

```text
NODE_ID
HAZARD_TYPE
RISK_LEVEL
TIMESTAMP
LATITUDE
LONGITUDE
SENSOR_SUMMARY
BATTERY_STATUS
```

Example:

```text
NODE_ID      = NODE01
HAZARD       = FLOOD
RISK         = HIGH_RISK
TIME         = 2026-09-27 10:32:15
LATITUDE     = <GPS_LATITUDE>
LONGITUDE    = <GPS_LONGITUDE>
WATER_LEVEL  = <VALUE>
RAINFALL     = <VALUE>
BATTERY      = <VALUE>
```

## Communication Flow

```text
Node 1 ─┐
Node 2 ─┼── LoRa ──> Gateway ── Internet ──> Backend
Node 3 ─┘                                      |
                                               |
                                  +------------+------------+
                                  |                         |
                                  v                         v
                              Mobile App              Web Dashboard
```

## Note

The prototype uses LoRa wireless communication.

LoRaWAN should only be claimed if a LoRaWAN network architecture and
stack are actually implemented.
