# PressureX Sensor – Radiation Exposure Test Protocol

**Version:** 1.1  
**Date:** 2025-05-17  
**Author:** Bryce Lovell  
**Target Audience:** Reliability / Radiation Test Engineers  

---

## Objective
Prototype-level radiation exposure planning protocol to evaluate:
- Total Ionizing Dose (TID) response
- Single Event Effects (SEE) susceptibility (if applicable)
- Drift/degradation relative to baseline

This is a **planning template** and does **not** imply compliance or facility access.

---

## References (examples only)
Listing here does **not** imply compliance:
- JEDEC JESD89 (SEE methodology) (as applicable)
- MIL-STD-883 Method 1019 (TID) (as applicable)
- ECSS radiation/environment standards (as applicable)

---

## Facility Requirements (generic)
Use a qualified facility capable of:
- Controlled TID exposure (gamma or equivalent)
- SEE testing (proton/heavy ion) if required
- Dose measurement with traceable dosimetry

---

## Sensor Preparation
- **Configuration:** As-built prototype configuration
- **Biasing:** Define powered vs unpowered exposure per plan
- **Monitoring:** Define sample rate and logged channels
- **Shielding:** Define “none” or specify thickness/material if included

---

## Test Plan Overview

### A) Total Ionizing Dose (TID) (example framework)
| Parameter     | Example Value (adjust) |
|---------------|-------------------------|
| Dose Rate     | Define per facility/program |
| Total Dose    | Define per environment/program |
| Duration      | Derived from dose + rate |
| Sensor State  | Powered or unpowered (define) |

- Record baseline and in-exposure performance
- Track drift, offset changes, or functional errors

### B) Single Event Effects (SEE) (optional)
| Parameter     | Example Value (adjust) |
|---------------|-------------------------|
| Particle Type | Proton or heavy ion (define) |
| Energy/LET    | Define |
| Flux          | Define |
| Duration      | Define |

- Monitor for upsets, latch-ups, or resets
- Log anomalies with timestamps and exposure conditions

---

## Proposed Pass/Fail Criteria (Prototype)
Define per mission/use-case; common criteria include:
- No destructive latch-up or permanent failure
- Drift remains within defined tolerance relative to baseline
- Recovery behavior is deterministic and logged (reset/watchdog as designed)

---

## Post-test
- Power-cycle and functional retest
- Visual inspection (PCB, housing, connectors)
- Archive raw logs + metadata under a results folder (if/when run)
