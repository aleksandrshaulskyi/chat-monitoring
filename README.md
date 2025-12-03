# Chat-monitoring.

Unified observability layer for the distributed chat platform

A dedicated monitoring microservice built on top of the modern OpenTelemetry → Prometheus → Grafana stack, providing real-time metrics, dashboards, and operational visibility for all backend services in the system.

## 🚀 Overview

Chat-monitoring centralizes metrics collection, storage, and visualization for the entire distributed chat ecosystem.
It leverages a lightweight and production-grade observability stack:

**OpenTelemetry** — instrumentation & metric export

**Prometheus** — time-series database & scraping

**Grafana** — dashboards for real-time analytics

At the moment, the service tracks core, high-impact metrics such as:

**Requests per second (RPS)**

**p95 and p99 latency**

**Error-rate**

**WebSocket connection count (for the transport layer)**

This setup provides instant insight into system health, performance bottlenecks, and load patterns.

## 🧩 Features

Centralized metrics for all microservices
Each backend service exports standard OTel metrics that are scraped and visualized automatically.

Pre-provisioned Grafana dashboards
Includes three ready-to-use dashboards, one for every backend microservice:

- Chat-auth

- Chat-transport

- Chat-messaging

Vital performance metrics

Every dashboard includes:

- RPS

- p95 latency

- p99 latency

- Error-rate

**Transport-specific metrics**

For Chat-transport, an additional time series tracks the number of active WebSocket connections.

**Out-of-the-box Prometheus datasource**

Datasource provisioning included — no manual setup required.

**Batteries-included monitoring**

Instant local deployment with full observability stack running in Docker.

## ⚙️ Usage.

1) Clone the repository.
2) Create the .env file using the example in the root directory.
3) Switch to the directory that contains the docker-compose file.
4) Run ```docker-compose up --build```.
5) That is it. Access Grafana on **http://localhost:3030**

## 🔗 Back to the Main Index Repository

Explore the full distributed chat system:
https://github.com/aleksandrshaulskyi/chat-index
