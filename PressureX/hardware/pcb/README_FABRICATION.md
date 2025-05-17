# PressureX PCB Fabrication & Assembly Notes

## Overview
This document contains guidelines for fabricating and assembling the PressureX PCB, designed to support a BMP388 sensor and STM32F103C8T6 MCU for high-resolution barometric pressure measurement in aerospace environments.

---

## PCB Specifications

| Parameter                  | Value                  |
|---------------------------|------------------------|
| Dimensions                | 30mm x 20mm            |
| Layers                    | 2                      |
| Copper Thickness          | 1 oz                   |
| Board Thickness           | 1.6mm                  |
| Surface Finish            | ENIG (Gold)            |
| Soldermask Color          | Black                  |
| Silkscreen Color          | White                  |
| Min Trace Width/Spacing   | 6 mil                  |
| Drill Size (Via)          | 0.4mm                  |
| Via Type                  | Through-hole           |
| Edge Cuts Tolerance       | ±0.1mm                 |

---

## Recommended Fabrication House

Any IPC Class 2 certified PCB manufacturer with ENIG capability is acceptable. Recommended examples:
- JLCPCB
- OSH Park
- PCBWay

---

## Assembly Notes

### Components:
- **U1**: STM32F103C8T6 (LQFP-48)
- **U2**: Bosch BMP388 sensor (QFN)
- Standard 0603 or 0402 passives for pull-ups, decoupling caps

### Assembly Process:
1. Use reflow soldering for QFN and LQFP components. Manual soldering of passives is acceptable.
2. Use stencil for solder paste application (recommended thickness: 0.12mm).
3. Bake assembled boards at 120°C for 2 hours to remove moisture before use in vacuum or thermal cycling environments.

---

## Testing & QA

Post-assembly validation checklist:
- ✔ Power continuity (3.3V and GND)
- ✔ I²C communication test with BMP388
- ✔ SWD interface check with STM32
- ✔ No shorts or lifted pads under QFN sensor

---

## Notes for Space Use

- Apply conformal coating if exposure to moisture or contaminants is likely.
- Consider potting the sensor if shock/vibration exceed 50g.
- If flying to orbit: all components must be space-grade or radiation-tolerant.

---

## Gerber & Assembly Files

> [COMING SOON: Will be added in `/hardware/pcb/fab_files/` folder]

---

## Maintainer

Bryce W.  
[https://github.com/BryceWDesign]

---
