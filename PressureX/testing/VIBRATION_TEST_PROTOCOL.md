# Vibration Test Protocol for PressureX Hardware

## Purpose

To verify that the PressureX sensor assembly and PCB hardware can withstand the mechanical stresses of launch and operation in space environments.

---

## Test Setup

- **Test Item:** Fully assembled PressureX sensor PCB with mounting hardware  
- **Fixture:** Vibration table with mounting fixture replicating flight mounting points  
- **Instrumentation:** Accelerometers mounted on test item and fixture  
- **Data Acquisition:** High-speed data logger for acceleration and frequency response

---

## Test Conditions

| Axis       | Frequency Range | Sweep Rate     | Acceleration (g RMS) | Duration         |
|------------|-----------------|----------------|---------------------|------------------|
| X (long)   | 20 Hz - 2000 Hz | 2 oct/min      | 14.1 g RMS          | 120 seconds      |
| Y (lat)    | 20 Hz - 2000 Hz | 2 oct/min      | 14.1 g RMS          | 120 seconds      |
| Z (vert)   | 20 Hz - 2000 Hz | 2 oct/min      | 14.1 g RMS          | 120 seconds      |

---

## Test Procedure

1. Mount the test item securely to the vibration table fixture.  
2. Attach accelerometers at critical points on the PCB and sensor housing.  
3. Perform a pre-test visual inspection and functional test.  
4. Run vibration sweep on X-axis as specified.  
5. Run vibration sweep on Y-axis as specified.  
6. Run vibration sweep on Z-axis as specified.  
7. After each axis test, perform functional check and visual inspection.  
8. Document any anomalies or failures.

---

## Acceptance Criteria

- No physical damage or component loosening.  
- No significant degradation in sensor functionality or signal quality.  
- No trace or pad damage on PCB.

---

## Reporting

Record test results, including accelerometer data, visual inspection findings, and functional test results, in the Test Results Log.

---

*End of Vibration Test Protocol*
