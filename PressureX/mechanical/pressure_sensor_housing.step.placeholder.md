# Pressure Sensor Housing (CAD Placeholder)

> **Status:** Placeholder notes. A real STEP export is **not** currently included.

Actual STEP files can be ASCII (ISO-10303-21) or binary; this repo currently stores interface assumptions in text so reviewers can see intended geometry.

## Concept specs
- Outer dimensions: 50 mm x 40 mm x 20 mm (L x W x H)
- Material: aluminum alloy (e.g., 6061-T6) selected per environment/requirements
- Wall thickness: 3 mm
- Mounting holes: 4x M3 threaded holes, 35 mm spacing (center-to-center)
- Sensor cavity: sized to fit PCB and sensor module securely
- Cable entry: gland or sealed grommet (define per environment)

## To create a real CAD export
Create the model in CAD (SolidWorks/Fusion 360/FreeCAD, etc.) and export:
- `pressure_sensor_housing.step`

Then remove/replace this placeholder.
