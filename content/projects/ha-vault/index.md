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

Engineered a **high-availability HashiCorp Vault cluster** backed by **Consul** and secured behind a **multi-stage NGINX reverse proxy**. Designed to ensure resilient secret management, **encrypted communication**, and **identity-based access control** across distributed services.

This project emphasized **redundancy**, **fault tolerance**, and secure secret governance.

---

## Architecture

- **Vault** deployed in **server mode**
- **Consul** backend for **HA storage**
- **Shamir secret sharing** initialization
- **Reverse proxy** architecture with **SSL/TLS**
- Controlled **container networking**
- **Root** and **userpass** authentication methods enabled

Vault nodes operate in **active/standby** mode to maintain availability.

---

## Security Controls

- **Unseal threshold enforcement** (Shamir)
- **Role-based access policies**
- **Encrypted inter-node communication**
- **Reverse proxy isolation** from direct access
- **Token-based** and **userpass** authentication

---

## Key Outcome

Deployed a resilient **secret management platform** capable of maintaining continuity while enforcing **identity-based controls** and secure access paths.

---

## Vault Cluster Status (Active Node)

![Vault Active](/images/projects/ha-vault.png)

---

## Architecture Flow

![Flow Diagram](/images/projects/traffic.png)