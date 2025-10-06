---
title: Clift Home Lab
description: 
published: true
date: 2025-10-06T21:27:31.141Z
tags: homelab
editor: markdown
dateCreated: 2025-01-30T04:25:04.642Z
---

## Design
- The overall design of the home lab is to run a mini K8s instance, Microk8s is the flavor there are 2 Clusters 1 for homelab and one for Runway which operates the house.

- Most services are available via the homepage setup on the cluster available at https://dashy.network-gnomes.com

- Other services are avaialbe usually only as a temporary service or services that dont require direct user interaction. They can be obtained by logging into the cluster and issuing the commands.
`sudo microk8s kubectl describe ing -n homelab ingress-network-gnomes.com`

## Hardware
- Below is a list of hardware click on the specific devices to view more details about the device.
### Servers
- **[Whitemage](/HomeLab/Hardware/whitemage):**
  - **Model:** Orange Pi 5
  - **Role:** Control-Plane
  - **Ip Address:** 172.25.75.74

- **Blackmage:**
  - **Model:** Orange Pi 5
  - **Role:** Worker
  - **Ip Address:** 172.25.75.75

- **Bluemage:**
  - **Model:** Orange Pi 5
  - **Role:** Kubernetes Cluster 2 (RUNWAY Primary)
  - **Ip Address:** 172.25.75.76

### Networking Equipment
- **Router:**
  - **Model:** Unifi Security Gateway
  - **Ip Address:** 172.25.15.1

- **Switch:**
  - [Unifi 24 Non PoE](/HomeLab/Hardware/unifi48)
    - **Model:** USW-24-Pro
    - **Ports:** 24 See Port Map on the switch
  - Unifi 24 POE
    - **Model:** US 24 PoE 250w
    - **Ports:** 24
  - Zytel 24 Port Video Distrabution
    - **Model:** Zytel 24 Port
    - **Ports:** 24