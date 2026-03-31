# Lesson 5: Home Network Documentation

**Author:** Git-Fama  
**Date:** March 2026  
**Project Scope:** Documentation of a two-story residential network (Basement Tenant Perspective).

---

## 1. Physical and Logical Topologies

### Physical Topology
This diagram illustrates the physical distribution of devices. The network originates from the main floor (landlord's area) and extends to the basement via wireless signals.

![Physical Topology](./images/physical_topology.png)

### Logical Topology
The logical structure shows the data flow and addressing hierarchy. All basement devices are part of a single flat subnet managed by the primary gateway.

![Logical Topology](./images/logical_topology.png)

---

## 2. Addressing & Device Inventory

This table provides detailed information on all active network devices, their roles, and connection types.

| Device Name | Brand/Model | Connection Type | Assigned IP (DHCP) | Network Role |
| :--- | :--- | :--- | :--- | :--- |
| **Main Router** | Unknown (Landlord) | Fiber/WLAN | 192.168.1.1 | Default Gateway |
| **Desktop PC** | Custom Built | Wi-Fi 6 (802.11ax) | 192.168.1.10 | Primary Workstation |
| **Smartphone 1** | OPPO Find X7 Ultra | Wi-Fi 6 | 192.168.1.11 | Mobile Device |
| **Smartphone 2** | Samsung S23+ | Wi-Fi 6 | 192.168.1.12 | Mobile Device |
| **Smartphone 3** | Redmi Note 12 Turbo| Wi-Fi 5 | 192.168.1.13 | Mobile Device |
| **Tablet** | iPad Pro M1 | Wi-Fi 6 | 192.168.1.14 | Productivity |
| **Game Console** | Nintendo Switch | Wi-Fi 5 | 192.168.1.15 | Entertainment |
| **Smart Home** | Mi Air Purifier 4S | Wi-Fi 2.4GHz | 192.168.1.16 | IoT Device |

---

## 3. Network Services

- **DHCP & NAT:** Managed by the main router to provide dynamic addressing and internet access.
- **File Sharing (SMB):** Enabled on the Desktop PC for local network data transfer.
- **Cloud Services:** Devices sync data via iCloud (iPad) and Mi Home (Air Purifier).

---

## 4. Device Configurations

Due to administrative restrictions as a tenant, access to the primary router's command-line interface (CLI) is unavailable. However, the workstation (Desktop PC) configuration is as follows:

- **OS:** Windows 11 Pro
- **NIC:** Wi-Fi 6 Wireless Network Adapter
- **IP Assignment:** Automatic (DHCP)
- **Primary DNS:** 192.168.1.1 (Gateway forwarder)
- **Local Security:** Active Windows Defender Firewall and periodic antivirus scanning.

*Note: For privacy, MAC addresses have been omitted from the inventory table.*

---

## 5. Credential Management & Security

**Storage Method:**  
For my home network, I securely store all passwords and service credentials using the **Microsoft Edge built-in password manager**. This ensures that my credentials stay encrypted and synchronized across my PC and mobile devices.

**Security Policy:**
- **No Shared Accounts:** I maintain a unique local administrator account for my PC and do not share any credentials with other tenants in the household.
- **Password Strategy:** Each service (Xiaomi Home, Nintendo, Samsung) uses a high-entropy, unique password to prevent cross-account security risks on a shared network.

---
*Created as part of the MITT-NSA-SOP Assignment.*
