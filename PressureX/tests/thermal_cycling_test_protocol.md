# PressureX Sensor – Thermal Cycling Test Protocol

**Document Version:** 1.0  
**Date:** 2025-05-17  
**Author:** B. W. Design  
**Target Audience:** QA Engineers, Mission Assurance Teams, Aerospace Test Facilities  

---

## Objective

To assess the PressureX sensor’s performance and structural stability when subjected to repeated temperature extremes simulating Low Earth Orbit (LEO) and deep space environments.

---

## Test Equipment Required

- Thermal chamber (range: -60°C to +120°C)
- Digital temperature logger
- DAQ system with serial/USB input
- Insulated test fixture with thermal break
- Reference pressure source (optional for calibration drift check)

---

## Sensor Test Configuration

- **Mounting:** Sensor secured to aluminum plate with thermal pads
- **Power:** 3.3V from external lab PSU
- **Interface:** USB or UART connection to host DAQ
- **Data Logging:** Live sensor data captured at 1Hz throughout cycling

---

## Procedure

### 1. Pre-Test Baseline

- Functional test at room temperature (20°C)
- Record pressure reading output baseline
- Document firmware version and serial number

### 2. Thermal Cycling Parameters

| Phase | Temperature | Soak Time | Transition Time |
|-------|-------------|-----------|-----------------|
| 1     | +85°C       | 30 min    | ≤10 min         |
| 2     | -40°C       | 30 min    | ≤10 min         |

- **Cycle Count:** Minimum 10 full thermal cycles
- Total test time: ~12 hours including transitions
- Data recorded throughout entire cycle

---

## Pass/Fail Criteria

- No deviation > ±3% in pressure readings from baseline
- No physical warping or housing fractures
- No communication interruptions or resets
- No solder joint failure (verified by post-test continuity check)
- Sensor reboots and functions within 5s post-cycle

---

## Post-Test Actions

- Visual inspection and high-resolution photography
- Data file archive (CSV or JSON)
- Functional re-validation under nominal conditions
- File results under `tests/results/thermal/` directory

---

## Notes

- Optional: Extend test to 100 cycles for deep space mission profiles
- Document any condensation-related issues or material fatigue
- Consider conformal coating revision if failure occurs

---
