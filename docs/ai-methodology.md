# AI / Edge Intelligence Methodology

## Objective

The system performs local analysis of multiple sensor parameters to
identify abnormal environmental conditions and classify the risk level.

## Multi-Sensor Fusion

Instead of using a single sensor value, the system considers multiple
parameters associated with each hazard.

---

## Flood

Inputs:

- Water Level
- Rainfall
- Temperature
- Humidity
- Rate of Water-Level Change

Concept:

```text
Water Level
Rainfall
Temperature
Humidity
Rate of Change
      ↓
Feature Processing
      ↓
Risk Analysis
      ↓
Normal / Warning / High Risk / Danger
```

---

## Forest Fire

Inputs:

* Temperature
* Humidity
* Smoke
* Gas concentration
* Flame indication

Concept:

```text
Temperature
Humidity
Smoke
Gas
Flame
  ↓
Feature Processing
  ↓
Risk Analysis
  ↓
Normal / Warning / High Risk / Danger
```

---

## Landslide

Inputs:

* Soil Moisture
* Ground Movement / Tilt
* Vibration
* Rainfall
* Temperature
* Humidity

Concept:

```text
Soil Moisture
Ground Movement
Vibration
Rainfall
  ↓
Feature Processing
  ↓
Risk Analysis
  ↓
Normal / Warning / High Risk / Danger
```

---

## Edge Processing

Initial processing is performed locally on the ESP32-S3.

This reduces dependency on continuous Internet connectivity and allows
faster local detection.

## Important Implementation Note

The exact machine-learning model, trained weights and deployment method
will be documented here once the model is finalized and deployed on
the ESP32-S3.

The system architecture supports lightweight edge-AI/risk-classification
models.
