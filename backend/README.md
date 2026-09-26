# Backend / Cloud

## Purpose

The backend receives processed information from the gateway and makes
the information available to the mobile application and web dashboard.

## Main Responsibilities

- Receive node data
- Store environmental data
- Store alerts
- Store node locations
- Store timestamps
- Maintain node status
- Provide APIs
- Send notifications
- Provide historical information

## Data Flow

```text
Gateway
   ↓
Backend API
   ↓
Database
   ↓
 ┌───────────────┐
 │               │
 ▼               ▼
Mobile App   Web Dashboard
```

## Example API Structure

```text
GET  /api/nodes
GET  /api/nodes/{id}
GET  /api/alerts
GET  /api/alerts/{id}
GET  /api/history/{nodeId}
POST /api/telemetry
POST /api/alerts
```

## Note

Replace these example endpoints with the actual backend endpoints once
the backend is implemented.
