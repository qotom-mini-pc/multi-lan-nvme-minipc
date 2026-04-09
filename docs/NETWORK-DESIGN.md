# Network Design (Multi-LAN Architecture)

## Overview

This platform uses multiple physical NICs to separate network traffic instead of relying only on VLANs.

It is designed for mixed workloads such as:

- NAS (storage traffic)
- client network (LAN)
- routing / firewall (WAN)

---

## Typical Topology
Internet
|
[WAN]
|
pfSense / Router
| | |
LAN NAS MGMT
| | |
PCs Storage Admin

---

## Interface Assignment

Example:

- WAN → Internet access
- LAN → client devices
- NAS → storage traffic
- MGMT → management / services

---

## Multi-LAN vs VLAN

### Multi-LAN (Physical Separation)

Advantages:

- Dedicated bandwidth per interface
- Reduced traffic interference
- Easier troubleshooting

Disadvantages:

- More cabling
- Requires more switch ports

---

### VLAN (Logical Separation)

Advantages:

- Flexible configuration
- Fewer physical interfaces required

Disadvantages:

- Shared bandwidth
- Depends on switch performance

---

## Design Notes

- Multi-LAN is beneficial when NAS traffic is heavy
- Separating storage traffic improves responsiveness
- Can be combined with VLANs if needed

---

## Use Cases

- NAS + router combined systems
- homelab environments
- edge computing nodes
