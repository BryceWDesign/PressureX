# PressureX Sensor – Radiation Exposure Test Protocol

**Version:** 1.0  
**Date:** 2025-05-17  
**Author:** B. W. Design  
**Target Audience:** Aerospace Radiation Testing Facilities, Reliability Engineers

---

## Objective

To evaluate the PressureX sensor’s resistance to radiation typically encountered in Low Earth Orbit (LEO) and Geostationary Earth Orbit (GEO) missions, focusing on:

- Total Ionizing Dose (TID)
- Single Event Effects (SEE)
- Cumulative performance degradation

---

## Applicable Standards

- NASA EEE-INST-002
- ESA ECSS-Q-ST-60-15C
- JEDEC JESD89A

---

## Radiation Test Facilities

Suggested certified labs:

- NASA Goddard Radiation Effects Facility
- ESA/ESTEC Test Centre
- TRIUMF (Canada)
- Brookhaven National Laboratory (BNL)

---

## Sensor Preparation

- **Encapsulation:** As in flight-ready configuration
- **Biasing:** Sensor powered and transmitting data during exposure
- **Monitoring:** Pressure output sampled at 2Hz
- **Shielding:** None unless otherwise specified

---

## Test Plan Overview

### A. Total Ionizing Dose (TID)

| Parameter     | Value             |
|---------------|------------------|
| Dose Rate     | 50–300 rad(Si)/hr |
| Total Dose    | 20 krad(Si)       |
| Duration      | ~72 hrs           |
| Sensor State  | Active            |

- Record real-time sensor performance
- Identify offset drift or functional errors

---

### B. Single Event Effects (SEE)

| Parameter         | Value              |
|-------------------|-------------------|
| Particle Type     | Heavy Ions         |
| LET Range         | 5–60 MeV·cm²/mg    |
| Flux              | ~10⁵ ions/cm²·s    |
| Test Duration     | 30–60 min/LET step |

- Monitor for bit flips, latch-up, or resets
- Log all anomalies with timestamp and LET

---

## Pass/Fail Criteria

- Functional within 5% accuracy drift post-TID
- No destructive latch-up or unrecoverable SEE
- Self-recovery or watchdog response to SEU

---

## Post-Test Procedure

- Power cycle and reboot tests
- Full functionality retest at room temperature
- Visual inspection of PCB, sensor housing
- Submit all logs and metadata under:
  `tests/results/radiation_exposure/`

---

## Recommendations

- Consider radiation-hardened components for future rev
- Shielding optimization may be required for >20krad missions
- Update conformal coating to meet MIL-STD-883 if failures observed

---
