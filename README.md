# Enterprise Campus Network Design using Cisco Packet Tracer

## Overview

This project demonstrates the design and implementation of a fully redundant three-tier enterprise campus network using Cisco Packet Tracer.

The network follows industry-standard hierarchical architecture with Core, Distribution, and Access layers. The implementation includes VLAN segmentation, inter-VLAN routing, OSPF dynamic routing, HSRP gateway redundancy, and STP loop prevention.

---

# Network Architecture

## Core Layer
- CORE1
- CORE2

## Distribution Layer
- DIST1
- DIST2

## Access Layer
- ACC1
- ACC2
- ACC3
- ACC4

---

# Technologies and Protocols Used

- Cisco Packet Tracer
- VLANs
- Inter-VLAN Routing
- OSPF
- HSRP
- PVST (Spanning Tree Protocol)
- Layer 3 Switching
- 802.1Q Trunking

---

# VLAN Design

| VLAN | Department |
|------|------------|
| 10   | HR         |
| 20   | FINANCE    |
| 30   | IT         |
| 40   | GUEST      |

---

# Features Implemented

- VLAN Segmentation
- Inter-VLAN Routing
- Dynamic Routing using OSPF
- HSRP Gateway Redundancy
- STP Root Bridge Optimization
- Dual Core Redundancy
- Distribution Layer Redundancy
- Access Layer Redundant Uplinks
- Failover Testing

---

# HSRP Design

| VLAN | Active Switch |
|------|---------------|
| VLAN 10 | DIST1 |
| VLAN 20 | DIST2 |
| VLAN 30 | DIST1 |
| VLAN 40 | DIST2 |

---

# STP Root Bridge Design

| VLAN | Root Switch |
|------|-------------|
| VLAN 10 | DIST1 |
| VLAN 20 | DIST2 |
| VLAN 30 | DIST1 |
| VLAN 40 | DIST2 |

---

# Verification Commands

## OSPF
```bash 
```bash
show ip ospf neighbor
show ip route
```

## HSRP
``` bash
show standby brief
```
``` 
```
```

```
## STP
```bash 
show spanning-tree
show spanning-tree vlan 10
```

## Trunk
```bash
show interfaces trunk
```


```
```

# Future Improvements

- EtherChannel
- ACL Security Policies
- DHCP Server
- Port Security
- DHCP Snooping
- Syslog Monitoring



