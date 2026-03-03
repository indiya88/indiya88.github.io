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

Designed a secure, containerized observability architecture using **NGINX reverse proxies** with automated **SSL/TLS termination**.  

Deployed a **Loki–Grafana stack** integrated with **Fluent Bit sidecars** to centralize log aggregation, analyze system behavior, and transform infrastructure telemetry into actionable operational insights.

---

## Key Components

- NGINX reverse proxy with TLS termination  
- Loki centralized log storage  
- Grafana dashboards for system monitoring  
- Fluent Bit log shipping and parsing  

---

## Architecture

![Architecture](architecture.png)

---

## Log Exploration Example

![Grafana Logs](grafana.png)