# SIH26178 – Problem Statement

## Title

A resilient, AI-powered environmental monitoring network that provides
early detection, localized intelligence, and actionable alerts for
floods, forest fires, pollution events, and other environmental hazards
common in India, enabling authorities and communities to shift from
reactive disaster response to proactive risk prevention.

## Theme

Disaster Management

## Category

Hardware

## Problem

Environmental hazards can develop rapidly and affect remote or
vulnerable regions.

Traditional monitoring systems may depend on isolated measurements,
continuous connectivity, or centralized processing.

The proposed system addresses this challenge through distributed
intelligent monitoring nodes capable of local processing and
long-range communication.

## Proposed Approach

The system uses multiple environmental sensors connected to ESP32-S3
controllers.

The nodes perform local data processing and risk classification before
sending compact information through LoRa to a gateway.

The gateway forwards the information to the backend/cloud platform,
which provides information to the mobile application and web dashboard.

## Target Hazards

1. Floods
2. Forest Fires
3. Air Quality / Pollution
4. Landslides
