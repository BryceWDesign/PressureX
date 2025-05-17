# Thermal Cycling Test Protocol for PressureX Sensor Assembly

## Objective

To assess the sensor assembly’s durability and performance across expected thermal extremes in space.

## Test Setup

- Place sensor assembly inside thermal chamber.
- Attach temperature sensors to critical points.
- Power and monitor sensor output continuously.

## Temperature Cycle

| Step      | Temperature (°C) | Duration         | Ramp Rate (°C/min) | Notes                   |
|-----------|------------------|------------------|--------------------|-------------------------|
| 1         | -40              | 1 hour           | 5                  | Simulate cold space temp|
| 2         | +85              | 1 hour           | 5                  | Simulate hot sun exposure|
| 3         | Repeat steps 1-2 | 10 cycles total  |                    |                         |

## Acceptance Criteria

- No mechanical damage or seal degradation.
- Sensor readings remain stable within calibration range.
- No condensation inside enclosure.

## Reporting

- Visual inspection pre- and post-test.
- Continuous logging of sensor data.
- Summary report with pass/fail results.

---

Reference: NASA-STD-7001 for space hardware thermal cycling.

