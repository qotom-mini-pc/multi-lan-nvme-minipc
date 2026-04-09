# Thermal Behavior

## Overview

Compact systems with multiple NICs and NVMe drives generate sustained heat under load.

---

## Heat Sources

- CPU
- NVMe SSDs
- network controllers

---

## Observations

- NVMe temperature rises quickly under heavy writes
- CPU temperature is generally stable
- airflow is the key factor

---

## NVMe Behavior

- without cooling → throttling may occur (~70–80°C)
- with airflow → stable performance

---

## Cooling Recommendations

- ensure airflow across SSDs
- avoid blocking vents
- consider thermal pads

---

## Fan Behavior

- fan curve affects stability
- higher airflow improves sustained performance
- balance noise vs cooling

---

## Monitoring Tools

- lm-sensors
- smartctl
- system logs

---

## Key Points

- NVMe is often the main heat source
- compact layout requires careful airflow design
- long-term stability depends on cooling

---

## Notes

Thermal performance varies with:

- ambient temperature
- workload intensity
- enclosure design
