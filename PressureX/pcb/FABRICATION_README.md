# PressureX PCB Fabrication Notes

This document provides essential information for fabricating and assembling the PressureX sensor PCB.

## PCB Specifications

- Board thickness: 1.6 mm (standard FR4)
- Copper thickness: 1 oz (35 µm)
- Surface finish: HASL Lead-Free
- Solder mask: Green, both sides
- Silkscreen: White on top and bottom
- Layer count: 2 (Top copper and Bottom copper)

## Drill and Via Information

- Standard drill size: 0.6 mm for pads
- Via drill size: 0.6 mm
- Via type: Through-hole plated vias
- Annular ring: Minimum 0.15 mm

## Component Placement

- Sensor IC footprint centered at (50 mm, 50 mm)
- 10-pin connector footprint at (70 mm, 50 mm)
- All surface mount pads are 1.5 x 1.5 mm
- Connector pads are through-hole with 1.0 mm drill

## Assembly Notes

- Use lead-free solder paste with reflow profile optimized for small SMD components
- Recommended stencil thickness: 0.1 mm stainless steel
- Hand soldering possible for connector pins, but automated pick-and-place recommended for SMD parts
- Verify polarity and orientation of the sensor IC before soldering

## Testing

- Electrical continuity test recommended after assembly
- Functional test by connecting to microcontroller with I2C lines (SDA, SCL) and power (VDD, GND)
- Check sensor output (OUT) pin with oscilloscope or ADC input

## Additional Notes

- Follow IPC-2221 standards for general PCB design guidelines
- Confirm footprint dimensions against component datasheets before fabrication
- This PCB is designed for aerospace environment; ensure quality controls per NASA/SpaceX standards

---

For any questions or clarifications, contact the design engineer.

