# PressureX PCB Fabrication Notes

## General

- PCB design created using KiCad version 7.0.
- Double-sided FR4 substrate, 1.6mm thickness.
- Copper thickness: 1 oz/ft² (35µm).
- Finish: ENIG (Electroless Nickel Immersion Gold) for corrosion resistance and space compatibility.

## Stackup

| Layer | Description           | Material                 | Thickness |
|-------|-----------------------|--------------------------|-----------|
| 1     | Top copper            | Copper foil              | 35 µm     |
| 2     | Prepreg               | FR4                      | 0.2 mm    |
| 3     | Core                  | FR4                      | 1.0 mm    |
| 4     | Bottom copper         | Copper foil              | 35 µm     |

## Special Instructions

- All vias must be plated through.
- Use thermal reliefs on pads connected to large copper pours.
- Solder mask: green, compliant with IPC-4101 Class 2.
- Silkscreen: white, for readability.
- Electrical test required after fabrication.
- Conformal coating recommended for space environmental protection (e.g., Parylene).

## Quality Control

- Follow IPC-A-600 Class 2 acceptance criteria.
- Include assembly fiducials as per drawings.
- PCB dimensions and hole sizes must comply with mechanical enclosure drawings.

---

Please coordinate with the fabricator for any questions or clarifications.

