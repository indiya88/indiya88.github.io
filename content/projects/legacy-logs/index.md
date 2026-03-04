---
title: "Zero-Trust Log Analytics Pipeline"
description: "Structured log ingestion pipeline, Fluent Bit, and Loki."
date: 2026-03-02
draft: false
tags: ["NGINX", "Loki", "Docker", "Security", "Log Analysis", "Zero Trust"]
# This hides the extra "Overview" card from your homepage
_build:
  list: never
  render: always
---

## Overview

Engineered a hardened **log analytics gateway** by isolating **Loki** behind an authenticated **NGINX reverse proxy**. Eliminated direct container exposure and enforced **access control** across all Loki API endpoints to implement a **zero-trust ingestion model**.

This project focused on securing the analytics pipeline itself.

---

## Security Architecture

- **Loki not publicly exposed** (no direct port publishing)
- **NGINX** as the **single access gateway**
- **Basic Authentication** enforced on:
  - `/loki/api/v1/push`
  - `/loki/api/v1/labels`
  - `/loki/api/v1/query`
  - `/loki/api/v1/series`
- Internal **Docker network isolation** restricting container communication
- No direct backend service access

All ingestion and queries must pass through **authentication enforcement**.

---

## Validation & Testing

- Verified enforcement using access logs:
  - Expected **401 Unauthorized** responses without valid credentials
- Confirmed all Loki requests were routed through **NGINX**
- Validated endpoint protection for both **push** and **query** paths

Validation confirmed through live NGINX access log monitoring (`docker exec -it nginx-logs tail -f /var/log/nginx/nginx-real.log`), where unauthorized requests returned **401** and authenticated requests returned **200 OK**.

---

## Analytics Impact

By securing ingestion endpoints, this design protects data integrity while enabling structured **log analysis** downstream (Grafana + Loki).

---

## Key Outcome

Implemented a **zero-trust enforcement layer** protecting the analytics pipeline, demonstrating **network segmentation**, **authenticated endpoints**, and security-first observability design.

---

## Log Query Example

![Log Query](/images/projects/nginx-logs.png)

---
