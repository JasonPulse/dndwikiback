---
title: Whitemage Info
description: 
published: true
date: 2025-10-06T21:05:53.284Z
tags: homelab, server, kubernetes
editor: markdown
dateCreated: 2025-10-06T21:05:53.284Z
---

# Server Name / Hostname

---

## 📝 Overview

* **Purpose:** Main machine for the homelab cluster
* **Location:** Where the machine is physically located (e.g., Office Rack, Basement).
* **Status:** `Online` / `Offline` / `Decommissioned`

---

## 🔩 Hardware Specifications

Orange PI 100gb, 32gig ram

---

## 💿 Software Configuration

### Operating System

* **OS:** Ubuntu Server 22.04
* **Key Roles:**
    * Microk8s Control Plane

### Key Applications / Services

* **Containerization:** Kubernetes (Microk8s)
* **Monitoring:** None
* **Backup:** None
* **Automation:** None

#### Running Configuration

Microk8s running Argocd
https://argocd.network-gnomes.com

ArgoCD automatically applys yaml files in the homelab github repo.

This system is built in a way that it can be blown away and the only setup required is to install argocd and link it to the github repo

After that will setup the individual services for the downloaders and indexers for prowlarr.  

Service access website can be located at
https://dashy.network-gnomes.com

---

## 🌐 Network Configuration

* **Hostname:** `whitemage`
* **Static IP Address:** 172.25.75.74
* **Cluster IP Address:** 172.25.75.70
* **MAC Address:** `AA:BB:CC:DD:EE:FF`
* **Connected Interface:** `eth0`
* **Key Open Ports:**
    * `22` (SSH)
    * `80` (HTTP)
    * `443` (HTTPS)

---

## 🛠️ Maintenance & Notes

### Backup Strategy

.... TODO....

### System Update Command

```bash
# For Debian/Ubuntu based systems
sudo apt update && sudo apt full-upgrade -y

# For Docker Compose containers
docker compose pull && docker compose up -d