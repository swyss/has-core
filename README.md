# 🧠 HAS Core

This repository contains the **core backend services** of the Home Automation System (**HAS**).  
It includes configuration, orchestration, authentication, internal messaging, logging, and OTA update infrastructure.

---

## 📦 Included Modules

- `Nucleus` – System kernel for configuration and service orchestration
- `Sentinel` – Authentication & Role Management (OAuth2/JWT)
- `CoreMesh` – Redis Streams-based internal messaging layer
- `DevControl` – Device registration, control and status interface
- `Beacon` – Alert manager for email, Telegram, and webhook notifications
- `NotifyX` – Real-time push service for WebSocket/WebPush/MQTT
- `LogStack` – Centralized structured logging with Loki/Filebeat
- `Pulse` – Prometheus-compatible system metrics exporter
- `FlashCast` – OTA firmware update service for ESP32/Arduino clients
- `SimulaX (backend)` – Integrated test and simulation backend

---

## 🚀 Features

- Centralized configuration and orchestration
- User and token management
- Internal service-to-service communication (event-based)
- Real-time notification and alerting
- OTA firmware update pipeline
- Metrics and log aggregation
- Simulation and testing backend support

---

## 🧱 Tech Stack

- Python, FastAPI, Alembic
- PostgreSQL, Redis (Streams & Sessions)
- Docker, MQTT
- Prometheus + Grafana, Loki
- PlatformIO (OTA tools)
- ASP.NET Core (SimulaX backend)

---

## 🛠️ Getting Started

```bash
git clone https://github.com/<your-username>/has-core.git
cd has-core
docker-compose up
