# Simulation README

## Purpose
This folder contains SPICE simulation files to validate the pressure sensor circuit design electrically before physical prototyping.

## Files
- `pressure_sensor_circuit_simulation.net`: SPICE netlist describing the sensor signal conditioning circuit.

## Requirements
- A SPICE simulator such as LTspice, NGSpice, or similar.
- Basic familiarity with running transient simulations in SPICE.

## How to Run
1. Open the `pressure_sensor_circuit_simulation.net` file in your SPICE simulator.
2. Run transient analysis for 10 milliseconds.
3. Observe the voltage waveform at nodes IN (sensor input) and OUT (post-conditioning output).
4. Validate that the output signal matches expected amplification and filtering characteristics.

## Notes
- This simulation models a simplified sensor and amplifier stage.
- Adjust component values in the netlist as needed to reflect final hardware specs.
- Simulation helps identify potential signal issues prior to PCB fabrication.

---

If you have questions or suggestions, feel free to open an issue.
