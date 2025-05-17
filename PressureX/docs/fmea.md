# Failure Modes and Effects Analysis (FMEA) for PressureX

| Component       | Failure Mode           | Effect of Failure                | Severity (1-10) | Cause of Failure                | Occurrence (1-10) | Detection (1-10) | Risk Priority Number (RPN) | Recommended Action                       |
|-----------------|-----------------------|--------------------------------|-----------------|-------------------------------|-------------------|-----------------|----------------------------|----------------------------------------|
| Pressure Sensor | Sensor signal loss     | Incorrect pressure reading     | 9               | Wiring failure, component fault| 3                 | 4               | 108                        | Add redundant signal path; regular calibration checks|
| PCB             | Trace break            | Sensor data loss               | 8               | Mechanical stress, manufacturing defects | 4        | 5               | 160                        | Use flex PCBs or strain relief; thorough inspection|
| Enclosure       | Seal failure           | Environmental contamination    | 10              | Material degradation, improper assembly | 2         | 6               | 120                        | Use space-grade sealing materials; assembly training|
| Firmware        | Data corruption        | Erroneous output readings      | 7               | Memory errors, software bugs   | 3                 | 3               | 63                         | Implement error checking and correction; thorough testing|
| Connectors      | Connection loss        | Loss of communication          | 8               | Vibration, connector wear      | 4                 | 5               | 160                        | Use locking connectors; vibration testing|

---

### Severity, Occurrence, and Detection Scale

- Severity: 1 (no effect) to 10 (catastrophic failure)  
- Occurrence: 1 (rare) to 10 (frequent)  
- Detection: 1 (easy to detect) to 10 (undetectable)  

---

The above RPN values highlight areas requiring prioritized mitigation to ensure reliable operation in space conditions.

