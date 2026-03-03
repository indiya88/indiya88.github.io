---
title: "From Legacy Logs to Centralized Observability"
description: "Structured log ingestion pipeline using Tomcat, Fluent Bit, and Loki."
date: 2026-03-02
draft: false
tags: ["Tomcat", "Fluent Bit", "Loki", "Grafana", "Log Parsing", "Data Analysis"]
# This hides the extra "Overview" card from your homepage
_build:
  list: never
  render: always
---

## Overview

Built a custom **Tomcat + Fluent Bit hybrid container** to capture, structure, and stream legacy Java application logs to a centralized **Loki** instance.

Implemented **TLS-encrypted streaming** and custom **regex parsing** to enable structured log analysis and improved visibility into system performance patterns.

---

## Log Query Example

![Log Query](grafana-query.png)

---

## Parsing Example

![Parsed Logs](parsed-logs.png)