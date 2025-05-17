# PressureX Thermal Cycling Test Protocol

## Objective

To assess the durability and operational stability of the PressureX sensor assembly under repeated thermal cycling between expected spacecraft temperature extremes.

## Test Setup

- Test chamber: Environmental thermal chamber capable of -40°C to +85°C  
- Sensor assembly mounted on vibration-isolated fixture  
- Instrumentation: Temperature sensors on housing and PCB, real-time sensor data acquisition

## Thermal Cycle Profile

| Cycle Step          | Temperature (°C) | Duration (minutes) |
|---------------------|------------------|--------------------|
| Start (ambient)      | 25               | 30                 |
| Cool-down ramp       | 25 to -40        | 60                 |
| Hold (cold soak)     | -40              | 120                |
| Warm-up ramp        | -40 to +85       | 90                 |
| Hold (hot soak)      | +85              | 120                |
| Cool-down ramp to ambient | 85 to 25     | 60                 |

- Number of cycles: 10 continuous cycles

## Pass/Fail Criteria

- No visible mechanical damage or cracking of housing or PCB  
- Sensor outputs remain stable and within specifications during and after testing  
- No intermittent electrical connections or signal degradation

## Procedure

1. Place sensor assembly in thermal chamber and connect data acquisition equipment.  
2. Program thermal chamber with cycle profile and start test.  
3. Monitor sensor data continuously through cycling.  
4. After completing 10 cycles, remove assembly and inspect for physical damage.  
5. Document all observations and test data.

## Safety and Precautions

- Ensure all equipment is rated for thermal cycling environment.  
- Avoid condensation damage by controlling ramp rates and humidity.  
- Follow lab safety protocols for handling extreme temperatures.

---

Reference: NASA-STD-7001A and MIL-STD-810G for thermal testing guidelines.

