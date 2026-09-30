# Web Dashboard

## Purpose

The web dashboard provides centralized monitoring of all environmental
monitoring nodes.

## Dashboard Features

- Live node monitoring
- Risk map
- Active alerts
- Sensor values
- Historical data
- Node health
- Battery information
- Event timeline
- Hazard filtering

## Dashboard Flow


```text
Nodes
  ↓
Gateway
  ↓
Backend
  ↓
Web Dashboard
  ↓
Authorities / Monitoring Team
```

## Planned Dashboard

```text
+------------------------------------------------+
| Environmental Monitoring Dashboard             |
+------------------------------------------------+
| Nodes | Alerts | Risk Map | History | Health   |
+------------------------------------------------+
|                                                |
|              RISK MAP                          |
|                                                |
|   🟢 Node 1      🔴 Node 2      🟡 Node 3      |
|                                                |
+------------------------------------------------+
| Active Alerts                                  |
|                                                |
| Flood     HIGH RISK     Node 1                 |
| Fire      WARNING       Node 2                 |
| Landslide NORMAL        Node 3                 |
+------------------------------------------------+
```
