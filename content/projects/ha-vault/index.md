---
title: "High-Availability Vault Architecture"
description: "HA HashiCorp Vault cluster backed by Consul with secure NGINX reverse proxy."
date: 2026-03-02
draft: false
tags: ["Vault", "Consul", "NGINX", "Security", "SSL/TLS", "HA Architecture"]
# This prevents the duplicate card from showing on the front page
_build:
  list: never
  render: always
---

## Overview

Engineered a high-availability **HashiCorp Vault** cluster backed by **Consul** and secured behind a multi-stage **NGINX reverse proxy** with SSL/TLS termination.

Implemented **Shamir seal initialization (5 shares, threshold 3)** and identity-based access controls to ensure secure secrets governance.

---

## Vault Cluster Status (Active Node)

![Vault Active](vault-active.png)

---

## Vault Cluster Status (Standby Node)

![Vault Standby](vault-standby.png)

---

## Architecture Flow

![Vault Architecture](architecture.png)