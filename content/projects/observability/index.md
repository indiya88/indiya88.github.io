---
title: "Zero-Trust Observability Pipeline"
description: "Secure, containerized observability stack using NGINX, Loki, Grafana, and Fluent Bit."
date: 2026-03-02
draft: false
tags: ["Docker", "NGINX", "Grafana", "Loki", "Fluent Bit", "Observability", "Log Analysis"]
# This prevents the duplicate card from showing on the front page
_build:
  list: never
  render: always
---

## Overview

Designed and deployed a **secure, containerized observability architecture** to centralize system telemetry and transform infrastructure logs into **actionable insights**. Implemented an **NGINX reverse-proxy gateway** with **SSL/TLS termination** and integrated **Fluent Bit sidecars** for structured log ingestion into **Loki**.

This project focused on building a resilient monitoring foundation while maintaining controlled access to log endpoints.

---

## Architecture

- **NGINX reverse proxy** with **SSL/TLS termination**
- **Fluent Bit sidecars** for log shipping
- **Loki** for centralized log aggregation
- **Grafana dashboards** for system monitoring
- **Docker network segmentation** between services

All external traffic is funneled through **NGINX** to prevent direct container exposure.

---

## Analytics Layer

- Structured log ingestion via **Fluent Bit**
- Centralized storage in **Loki**
- **Query-based log analysis** (Grafana Explore)
- **Real-time dashboards** in **Grafana**
- Infrastructure telemetry transformed into **operational insight**

---

## Log Exploration Example

Example Loki query:

- `{job="nginx"}`
- `{job="nginx"} |= "Authorization"`
- `{job="nginx"} |= "CustomUserAgent"`

(Insert your **Grafana Explore → Loki** screenshot here.)

---

## Key Outcome

Built a **secure observability pipeline** that balances **access control** with analytics, enabling insight without exposing backend services directly.

---

## Architecture

![Architecture](/images/projects/observe-pipe.png)

---

## Log Exploration Example

![Grafana Logs](/images/projects/nginx-logs.png)