# PressureX Vibration Test Protocol

## Objective

To verify the structural integrity and functional performance of the PressureX sensor assembly under simulated vibration conditions similar to launch and in-orbit environments.

## Test Setup

- Test fixture: Rigid mounting of sensor housing using custom clamp simulating spacecraft interface
- Instrumentation: Accelerometers attached to sensor housing and PCB
- Data acquisition: Real-time monitoring of sensor output signals and accelerometer data

## Vibration Profile

| Axis   | Frequency Range (Hz) | Acceleration (g) | Duration (minutes) |
|--------|---------------------|------------------|--------------------|
| X-axis | 20 - 2000           | 15               | 10                 |
| Y-axis | 20 - 2000           | 15               | 10                 |
| Z-axis | 20 - 2000           | 20               | 15                 |

- Sweep type: Sine sweep with random vibration overlay
- Test direction: Each axis tested independently, sequentially

## Pass/Fail Criteria

- No physical damage to sensor housing or PCB
- Sensor output signals remain within specification limits during and after test
- No loss of electrical continuity or intermittent connections

## Procedure

1. Mount sensor assembly securely in the vibration test fixture.
2. Connect instrumentation cables and verify data acquisition.
3. Apply vibration profile on the X-axis for the specified duration.
4. Monitor sensor signals and record data.
5. Repeat steps 3-4 for Y-axis and Z-axis.
6. Perform post-test inspection for mechanical and electrical integrity.
7. Document all results and deviations.

## Safety and Precautions

- Ensure all connections are secure to prevent damage.
- Use appropriate shielding to protect sensitive equipment.
- Follow lab safety protocols for vibration test equipment.

---

For further information, refer to NASA-STD-7001A for environmental testing standards.

