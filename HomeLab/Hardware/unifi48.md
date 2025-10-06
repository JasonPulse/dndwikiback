---
title: Unifi 48 Port Switch Map
description: output description for the unifi 48 port map
published: true
date: 2025-10-06T21:10:36.560Z
tags: homelab, hardware, switch
editor: markdown
dateCreated: 2025-10-06T21:10:36.560Z
---

# Switch Port Map: Unifi 48

---

## Switch Details

* **Model:** Ubiquiti USW-48
* **Location:** Office Rack
* **IP Address:** 192.168.1.2

---

## Port Assignments

| Port | Status | VLAN(s) | Connected Device | Notes |
|:----:|:------:|:-------:|:-----------------|:------|
| 1 | `UP` | 1 (Default) | `server-01` (eth0) | Primary server connection |
| 2 | `UP` | 1 (Default) | `server-02` (iDRAC) | Out-of-band management |
| 3 | `UP` | 10 (IoT) | `Living Room AP` | PoE+ enabled |
| 4 | `UP` | 20 (Cameras) | `Front Door Camera` | PoE enabled |
| 5 | `DOWN` | - | *Unused* | |
| 6 | `UP` | 1 (Default) | `Desktop PC` | |
| 7 | `DOWN` | - | *Unused* | |
| 8 | `UP` | 1 (Default) | `Uplink to Router` | Trunk Port (All VLANs) |
| ... | | | | |