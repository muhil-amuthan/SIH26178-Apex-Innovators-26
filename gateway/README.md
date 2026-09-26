# LoRa Gateway

The gateway receives environmental monitoring packets from the
distributed nodes.

## Data Flow

```text
Flood Node ──┐
Fire Node  ──┼──> LoRa Gateway
Landslide ───┘
                  ↓
               Internet
                  ↓
             Backend / Cloud
```

## Gateway Responsibilities

1. Receive LoRa packets.
2. Validate packet format.
3. Identify node.
4. Identify hazard.
5. Forward data to backend.
6. Handle communication errors.
7. Provide gateway health information.

## Example Packet

```json
{
  "node_id": "NODE01",
  "hazard": "FLOOD",
  "risk": "HIGH_RISK",
  "latitude": 0.0,
  "longitude": 0.0,
  "timestamp": "YYYY-MM-DD HH:MM:SS"
}
```
