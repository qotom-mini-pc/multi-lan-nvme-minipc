# Qotom Q31100G4 Mini PC – Multi-LAN + NVMe NAS / Router Platform

## Overview

This repository documents a compact **multi-LAN mini PC platform** based on the Qotom Q31100G4 series.

It is designed for combined workloads:

- NAS (network storage)
- Router / firewall (pfSense / OPNsense)
- Homelab services (Docker, edge computing)

Unlike traditional setups, this approach integrates **network + storage + services** into a single system.

---

## Hardware Features

Typical Q31100G4 configuration:

- 4 × Intel I226-V 2.5GbE LAN
- 4 × M.2 NVMe (PCIe Gen3)
- Intel Tiger Lake CPU (Celeron / i3 / i5)
- Dual DDR4 SO-DIMM

Available models:

- Q31111G4 – Celeron 6305 (low power NAS)
- Q31131G4 – Core i3-1115G4 (balanced)
- Q31151G4 – Core i5-1135G7 (multi-service workloads)

---

## Why Multi-LAN Mini PC for NAS

Traditional NAS systems:

- limited network interfaces
- SATA-based storage
- separate router required

This platform provides:

- multiple LAN ports for traffic separation
- NVMe storage for high I/O performance
- ability to run router + NAS on one device

---

## Typical Use Cases

- NAS server (TrueNAS / Unraid / OMV)
- Router / firewall (pfSense / OPNsense)
- Homelab environments
- Edge computing nodes
- Multi-service mini server

---

## Project Structure
docs/
configs/
benchmarks/
diagrams/

---

## Key Topics Covered

- Multi-LAN network design (vs VLAN)
- NVMe storage layout
- NAS + router combined deployment
- Performance observations
- Thermal behavior in compact systems
- Docker-based service stack

---

## Example Setup

- WAN → Internet
- LAN → client devices
- NAS → dedicated storage network

Storage:

- OS → NVMe
- Data → NVMe pool
- Cache → NVMe

---

## Why This Matters

Multi-LAN + NVMe mini PCs are increasingly used for:

- high-performance NAS
- compact homelab setups
- edge computing
- network appliances

This repository provides a practical reference for these use cases.

---

## Keywords

Qotom Q31100G4, mini PC NAS, multi LAN mini PC, 4 LAN router PC, homelab server, NVMe NAS, pfSense mini PC, fanless mini PC

---

## Notes

This is a system design and implementation reference, not a product advertisement.

Focus is on real-world usage, architecture, and performance behavior.
