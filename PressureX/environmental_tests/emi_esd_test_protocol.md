# EMI and ESD Test Protocol for PressureX Sensor Module

## Document Version
**Rev:** 1.1  
**Date:** 2025-05-17  
**Author:** Bryce Lovell

---

## Purpose
Define a **prototype-level** procedure and proposed acceptance criteria for Electromagnetic Interference (EMI) and Electrostatic Discharge (ESD) testing of the PressureX sensor module.

This document is provided as a **test template** for engineering review. It does **not** claim compliance or qualification to any specific program.

---

## Scope
Applies to the PressureX sensor PCB and enclosure assembly. Tests simulate electromagnetic disturbances and electrostatic events to verify device robustness and data integrity.

---

## References
The following are **example** reference documents commonly used for EMC planning. Listing a document here does **not** imply compliance.

- MIL-STD-461 (as applicable)
- IEC 61000-4-2 (ESD immunity)
- IEEE Std 299 (shielding effectiveness test methods)

---

## Test Setup

### Equipment Required
- EMI test chamber (shielded)
- Signal generator and spectrum analyzer
- ESD simulator (per IEC 61000-4-2)
- Test fixture replicating assembly with connectors and cabling

### Test Environment
- Temperature: 23°C ± 5°C
- Relative Humidity: 45% ± 10%

---

## Test Procedures

### EMI Testing
1. Place assembly inside EMI shielded chamber.
2. Power the device and run baseline sensor data capture.
3. Sweep frequency range 10 kHz to 18 GHz using signal generator (adjust to facility capability).
4. Monitor sensor output for deviations or dropouts.
5. Record anomalies exceeding baseline noise floor by a defined threshold (example: +3 dB).

### ESD Testing
1. Discharge ESD pulses at accessible points per IEC 61000-4-2.
2. Apply positive and negative discharges at 2 kV, 4 kV, 8 kV levels (or program-defined).
3. Verify functionality and data integrity after each discharge.
4. Repeat tests with device powered on and off.

---

## Proposed Acceptance Criteria (Prototype)
- No unintended reset, latch-up, or sustained data loss during exposure.
- Sensor output remains within an agreed tolerance band relative to pre-test baseline (define per use-case).
- No physical damage or permanent functional degradation observed post-test.

---

## Reporting
Document:
- Test conditions and environment parameters
- Pass/fail status for each level
- Observed anomalies or failures with timestamps and setup notes

---

## Remarks
Testing should be conducted under the supervision of a qualified EMC engineer. Use proper grounding/handling procedures to avoid damage.
