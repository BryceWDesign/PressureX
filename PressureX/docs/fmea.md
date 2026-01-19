# Failure Modes and Effects Analysis (FMEA) for PressureX (Prototype Instrumentation)

| Component       | Failure Mode           | Effect of Failure                | Severity (1-10) | Cause of Failure                          | Occurrence (1-10) | Detection (1-10) | Risk Priority Number (RPN) | Recommended Action |
|----------------|------------------------|----------------------------------|-----------------|-------------------------------------------|-------------------|------------------|----------------------------|-------------------|
| Pressure Sensor | Sensor signal loss     | Incorrect pressure reading       | 9               | Wiring failure, component fault            | 3                 | 4                | 108                        | Add redundant signal path; regular calibration checks |
| PCB            | Trace break            | Sensor data loss                 | 8               | Mechanical stress, manufacturing defects   | 4                 | 5                | 160                        | Add strain relief; inspect solder joints and vias; improve mounting/fixturing |
| Enclosure      | Seal failure           | Environmental contamination       | 10              | Material degradation, improper assembly    | 2                 | 6                | 120                        | Select seal materials appropriate to the intended environment; assembly training; leak check where applicable |
| Firmware       | Data corruption        | Erroneous output readings         | 7               | Memory errors, software bugs               | 3                 | 3                | 63                         | Implement error checking; watchdog/reset behavior; regression testing |
| Connectors     | Connection loss        | Loss of communication              | 8               | Vibration, connector wear                  | 4                 | 5                | 160                        | Use locking connectors; validate strain relief; verify contact retention post-test |

---

### Severity, Occurrence, and Detection Scale

- Severity: 1 (no effect) to 10 (catastrophic failure)  
- Occurrence: 1 (rare) to 10 (frequent)  
- Detection: 1 (easy to detect) to 10 (undetectable)  

---

This FMEA is a **prototype planning artifact** intended for review and iteration. It does not imply completed qualification.
