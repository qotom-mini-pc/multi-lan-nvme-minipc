# Deployment Example (NAS + Router + Services)

## Overview

This deployment combines:

- routing (pfSense / OPNsense)
- NAS storage
- container services

on a single compact system.

---

## Network Layout

- WAN → ISP
- LAN → clients
- NAS → storage network

---

## Storage Layout

- NVMe1 → OS
- NVMe2 → data
- NVMe3 → data
- NVMe4 → cache / logs

---

## Service Stack

- Router → pfSense / OPNsense
- NAS → TrueNAS / Unraid / OMV
- Containers → Docker

---

## Example Workflow

1. Internet traffic enters via WAN
2. Router handles routing/firewall
3. Clients access services via LAN
4. Storage traffic flows through dedicated NAS interface

---

## Advantages

- reduced network congestion
- improved storage performance
- compact deployment (all-in-one)

---

## Considerations

- thermal management is important
- proper NIC assignment required
- NVMe cooling may be needed
