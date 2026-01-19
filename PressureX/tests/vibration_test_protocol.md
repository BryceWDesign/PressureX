# PressureX Sensor – Vibration Test Protocol

**Document Version:** 1.1  
**Date:** 2025-05-17  
**Author:** Bryce Lovell  
**Target Audience:** Structures / Dynamics / Test Engineers  

---

## Objective
Prototype-level vibration test procedure for the PressureX sensor assembly to evaluate:
- Mechanical integrity (fasteners, housing, cable strain relief)
- Electrical continuity and functional data output pre/during/post test

This protocol is a **template**. It does **not** claim compliance with any specific customer/program standard.

---

## References (examples only)
Example documents commonly used to derive vibration environments. Listing here does **not** imply compliance:
- General Environmental Verification Standard (GEVS) style random vibration profiles (as applicable)
- MIL-STD environmental test methods (as applicable)

---

## Equipment Required
- Vibration table (3-axis shaker or equivalent)
- Data acquisition system (sample rate per sensor bandwidth; document actual)
- Accelerometers (range appropriate to expected levels)
- Test fixture (rigid mounting plate and hardware)
- Power supply (isolated, regulated)

---

## Test Configuration
- **Unit Under Test (UUT):** PressureX sensor assembly (as-built prototype)
- **Mounting:** Document bolt pattern, torque, and interface stack-up
- **Cabling:** Document routing and strain relief; avoid cable whip
- **Power/Data:** Document voltage, interfaces, and logging method

---

## Procedure

### 1) Pre-test checks
- Visual inspection (fasteners, solder joints, connectors)
- Continuity check
- Functional baseline capture (record baseline noise and nominal output)

### 2) Vibration sequence (define per environment)
Define axis-by-axis profiles per your target environment. Example framework:

| Axis | Profile Type | Frequency Range | Duration |
|------|--------------|-----------------|----------|
| X    | Sine sweep + random | Define | Define |
| Y    | Sine sweep + random | Define | Define |
| Z    | Sine sweep + random | Define | Define |

During each run:
- Log sensor output continuously
- Log accelerometer data at mounting interface
- Note any resets, dropouts, or connector intermittence

### 3) Post-test checks
- Re-run functional baseline capture
- Re-check continuity
- Inspect for cracks, loosening, connector damage, or wire fretting

---

## Proposed Pass/Fail Criteria (Prototype)
Define per use-case; common prototype criteria include:
- No physical damage or loose hardware
- No unintended reset or sustained data dropout
- Output remains within a defined tolerance band relative to pre-test baseline
- Post-test unit remains fully functional

---

## Data & Reporting
Record:
- Fixture drawing/photos + mounting torque
- Profile definitions + actual measured response
- Raw logs (sensor + accelerometers) + metadata (date, operator, SN)
