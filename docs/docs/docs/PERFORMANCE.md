# Performance Observations

## Overview

This document describes performance behavior under mixed workloads:

- network traffic
- storage I/O
- container services

---

## Test Environment

- 4 × 2.5GbE LAN
- 4 × NVMe SSD
- Intel CPU (i3 / i5 class)
- 16–32GB RAM

---

## Network Performance

- Single 2.5G link can reach near full bandwidth
- Multi-LAN improves traffic stability

Observations:

- NAS traffic separated from LAN reduces latency spikes
- concurrent transfers perform more consistently

---

## Storage Performance

NVMe layout:

- OS (dedicated)
- data drives
- cache

Observations:

- NVMe significantly outperforms SATA
- multiple drives reduce I/O contention
- mixed workloads run smoother

---

## CPU Behavior

- CPU usage is moderate under normal load
- higher usage when running:
  - encryption (VPN)
  - containers
  - heavy file operations

---

## Bottlenecks

- PCIe lane sharing
- NVMe thermal throttling
- network configuration

---

## Tools (Suggested)

- iperf3 → network testing
- fio → storage testing
- system monitoring tools

---

## Notes

Performance depends on:

- workload mix
- network design
- storage configuration
