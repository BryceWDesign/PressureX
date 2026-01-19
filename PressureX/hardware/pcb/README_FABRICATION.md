# PressureX PCB Fabrication & Assembly Notes (Prototype Instrumentation)

## Overview
Guidelines for fabricating and assembling the PressureX sensor PCB (BMP388 + STM32F103C8T6). This is **prototype instrumentation** intended to support validation workflows; it is **not flight-qualified**.

---

## PCB Specifications

| Parameter                | Value        |
|-------------------------|--------------|
| Dimensions              | 30mm x 20mm  |
| Layers                  | 2            |
| Copper Thickness        | 1 oz         |
| Board Thickness         | 1.6mm        |
| Surface Finish          | ENIG (Gold)  |
| Soldermask Color        | Black        |
| Silkscreen Color        | White        |
| Min Trace Width/Spacing | 6 mil        |
| Drill Size (Via)        | 0.4mm        |
| Via Type                | Through-hole |
| Edge Cuts Tolerance     | ±0.1mm       |

---

## Recommended Fabrication House
Any competent PCB manufacturer with ENIG capability is acceptable. Examples:
- JLCPCB
- OSH Park
- PCBWay

---

## Assembly Notes

### Components
- **U1**: STM32F103C8T6 (LQFP-48)
- **U2**: Bosch BMP388 sensor (QFN)
- Standard 0603/0402 passives for pull-ups and decoupling

### Assembly Process
1. Reflow recommended for QFN/LQFP components.
2. Stencil thickness: ~0.12mm (adjust as required).
3. If vacuum/thermal cycling is relevant, follow standard moisture handling practices for components/assemblies.

---

## Testing & QA (prototype)
- Power continuity (3.3V and GND)
- I²C communication with BMP388
- SWD interface check with STM32
- Visual inspection for shorts/lifted pads (especially under QFN)

---

## Environment Notes (select per use-case)
- Conformal coating can help with contamination/moisture exposure if relevant.
- Potting/encapsulation is optional and should be chosen based on the mechanical environment and serviceability needs.
- If radiation/vacuum/outgassing are in scope, select materials/components based on program requirements and verify via appropriate testing.

---

## Gerber & Assembly Files
If/when released, they should live alongside this README under a clearly versioned folder.

---

## Maintainer
Bryce Lovell  
https://github.com/BryceWDesign
