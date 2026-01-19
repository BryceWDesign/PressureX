# PressureX Sensor Housing (CAD Placeholder)

> **Status:** Placeholder notes. This repository does **not** currently include an exported STEP model for this part.

## Description
- Compact shell enclosure concept for sensor + PCB
- Suggested material: high-temperature engineering plastic or aluminum (select per environment and requirements)
- Pressure vent/port to allow external pressure communication (if required by use-case)

## Dimensions (concept)
- External: 35 mm (L) x 25 mm (W) x 15 mm (H)
- Wall thickness: 2 mm
- Internal cavity: fits 30 mm x 20 mm PCB
- Mounting tabs: 2x M2.5 screw holes on 30 mm spacing

## Features
- Pressure port: Ø2.5 mm (center-top)
- Lid concept with screw holes for retention
- Cable exit cutout: 5 mm x 3 mm

## Usage notes
- Select materials and sealing approach based on the intended environment (temperature, contamination, outgassing, serviceability).
- Verify tolerances and connector clearances in CAD prior to fabrication.

## To create a real CAD export
1. Create box: 35 x 25 x 15 mm
2. Shell: leave 2 mm wall thickness
3. Add top pressure port (Ø2.5 mm)
4. Add mounting tabs on bottom face
5. Cut internal pocket: 30 x 20 x 10 mm
6. Export the actual STEP file as `pressure_sensor_housing.step`

Then remove/replace this placeholder.
