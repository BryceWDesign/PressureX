# PressureX PCB Fabrication Notes (Prototype Instrumentation)

## General
- PCB design created using KiCad (version noted in repo history).
- FR4 substrate, 1.6mm thickness (unless otherwise specified).
- Copper thickness: 1 oz/ft² (35µm).
- Finish: ENIG (optional) for corrosion resistance and assembly robustness in harsher environments.

## Stackup (example)
| Layer | Description | Material | Thickness |
|-------|-------------|----------|-----------|
| 1     | Top copper  | Copper foil | 35 µm |
| 2     | Prepreg     | FR4         | 0.2 mm |
| 3     | Core        | FR4         | 1.0 mm |
| 4     | Bottom copper | Copper foil | 35 µm |

## Special Instructions
- All vias plated through.
- Thermal reliefs on pads connected to large pours.
- Solder mask: green (or specified), conforming to a typical IPC Class 2 process.
- Silkscreen: white.
- Electrical test recommended after fabrication.
- Conformal coating may be used for contamination/moisture protection where appropriate (select per environment).

## Quality Control
- Use IPC-A-600 Class 2 acceptance criteria as a general baseline (if applicable).
- Include assembly fiducials as per drawings.
- Verify PCB dimensions and hole sizes against the mechanical enclosure notes.

---
Coordinate with the fabricator for clarifications and ensure drawings/gerbers match the intended revision.
