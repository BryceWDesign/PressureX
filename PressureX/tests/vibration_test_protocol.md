# PressureX Sensor – Vibration Test Protocol

**Document Version:** 1.0  
**Date:** 2025-05-17  
**Author:** B. W. Design  
**Target Audience:** QA Engineers, Aerospace Contractors, Compliance Teams  

---

## Objective

To validate the structural integrity and electrical continuity of the PressureX sensor under simulated launch vibration profiles per NASA GEVS (GSFC-STD-7000A) and SpaceX payload qualification guidelines.

---

## Equipment Required

- Vibration Table (3-axis servo-hydraulic or electromagnetic shaker)
- Data Acquisition System (minimum 2kHz sampling)
- Accelerometers (±100g range)
- Test Fixture (aluminum mounting plate, M2 screws)
- Thermal Dummy Load (if heat dissipation is a factor)

---

## Sensor Test Configuration

- **Unit Under Test (UUT):** Fully assembled PressureX unit
- **Mounting Method:** 4x M2 bolts to aluminum fixture simulating onboard housing
- **Cable Management:** Sensor fully wired with ribbon cables; strain relief applied
- **Power:** Supplied via isolated 3.3V lab-grade source

---

## Procedure

### 1. Pre-Test Inspection

- Visual check for loose parts
- Electrical continuity check
- Functional boot-up via USB/serial output

### 2. Vibration Testing Sequence

| Axis        | Frequency Range | Sweep Rate | Duration per Axis |
|-------------|-----------------|------------|--------------------|
| X           | 20 Hz – 2 kHz   | 2 oct/min  | 10 min             |
| Y           | 20 Hz – 2 kHz   | 2 oct/min  | 10 min             |
| Z           | 20 Hz – 2 kHz   | 2 oct/min  | 10 min             |

- Test profile: Sine sweep and random vibration
- Random Profile Target: 14.1 Grms (NASA GEVS Class II payload)
- Peak Acceleration: 15g

---

## Pass/Fail Criteria

- No visual or structural damage
- Sensor output remains functional and within ±5% margin of baseline
- No mechanical detachment of internal components
- No connector decoupling or shorting
- Post-test full functionality (calibration check)

---

## Post-Test Actions

- Capture high-res photos for report
- Save log files from DAQ system
- Upload data to `tests/results/` with metadata (SN, date, operator)

---

## Notes

- Repeat test with thermal cycle preconditioning for combined stress validation
- Consider testing with vibration-damped PCB variant

---

