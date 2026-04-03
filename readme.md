# 🏠 Home Network Documentation

## 📌 Overview
This document provides a complete overview of my home network, including physical and logical topologies, IP addressing, network devices, configurations, and security practices.

---

## 🧠 Logical Topology

![Logical Topology](logical-topology.png)

### Description
The logical topology shows how devices communicate within the network.

### Devices:
- PC
- Laptop
- Tablet
- iPhone
- Smart TV
- Wireless Router

### Network Design:
- Star Topology (all devices connect to a central router)
- Router manages:
  - DHCP
  - NAT
  - Internet access

---

## 🖥️ Physical Topology

![Physical Topology](physical-topology.png)

### Description
The physical topology shows the actual placement of devices and connections.

### Device Locations & Connections

| Device      | Location        | Connection Type | Interface |
|------------|----------------|----------------|----------|
| Router     | Living Room     | ISP (WAN)       | WAN Port |
| PC         | Study Room      | Ethernet        | LAN Port 1 |
| Laptop     | Bedroom         | Wi-Fi           | Wireless |
| Tablet     | Bedroom         | Wi-Fi           | Wireless |
| iPhone     | Living Room     | Wi-Fi           | Wireless |
| Smart TV   | Living Room     | Wi-Fi           | Wireless |

### Cabling Details:
- Ethernet cable connects Router → PC
- Wireless connections for all other devices

---

## 🌐 Addressing Documentation

| Device      | IP Address      | MAC Address       | Type   |
|------------|----------------|------------------|--------|
| Router     | 192.168.1.1    | XX:XX:XX:XX:XX:01 | Static |
| PC         | 192.168.1.10   | XX:XX:XX:XX:XX:02 | DHCP   |
| Laptop     | 192.168.1.11   | XX:XX:XX:XX:XX:03 | DHCP   |
| Tablet     | 192.168.1.12   | XX:XX:XX:XX:XX:04 | DHCP   |
| iPhone     | 192.168.1.13   | XX:XX:XX:XX:XX:05 | DHCP   |
| Smart TV   | 192.168.1.50   | XX:XX:XX:XX:XX:06 | Static |

### Network Details:
- Network: `192.168.1.0/24`
- Default Gateway: `192.168.1.1`
- DNS: ISP provided

### Note:
- Static IP devices are assigned outside the DHCP range to prevent conflicts.

---

## ⚙️ Network Devices & Services

### 🔹 Router
The router is the central device in the network and performs:
- DHCP (Dynamic IP assignment)
- NAT (Private to Public IP translation)
- Firewall (Basic network security)
- Wireless access (Wi-Fi)

### 🔹 Services:
- DHCP Service
- NAT Service
- Wireless Networking (Wi-Fi)

---

## 🔧 Device Configurations

### Router Configuration:
- SSID: HomeNetwork
- Security: WPA2/WPA3 Personal
- DHCP Range: 192.168.1.10 – 192.168.1.100
- Default credentials changed

### PC:
- Connected via Ethernet
- Receives IP automatically (DHCP)
- Firewall enabled

### Laptop / Tablet / iPhone:
- Connected via Wi-Fi
- DHCP enabled
- Automatic network configuration

### Smart TV:
- Connected via Wi-Fi
- Configured with Static IP for stable connectivity
- Used for streaming services

---

## 🔐 Credential Security

To securely store login credentials, the following practices are used:

- Password Manager (e.g., Bitwarden / LastPass)
- Strong passwords (minimum 12 characters)
- Two-Factor Authentication (2FA)
- Default router username and password changed

---

## ✅ Conclusion

This documentation provides a clear and structured overview of the home network, including:

- Logical and Physical topology
- IP addressing scheme
- Device configurations
- Security best practices

The network is designed using a star topology with a centralized router, ensuring efficient communication and management.

---
