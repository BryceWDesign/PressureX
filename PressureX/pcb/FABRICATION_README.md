# PressureX PCB Fabrication Notes (Legacy / Reference)

This document provides legacy notes that were originally included with early sensor PCB drafts. Treat as **reference only** and verify against the actual PCB revision before fabrication.

## PCB Specifications
- Board thickness: 1.6 mm (standard FR4)
- Copper thickness: 1 oz (35 µm)
- Surface finish: HASL Lead-Free
- Solder mask: Green, both sides
- Silkscreen: White on top and bottom
- Layer count: 2

## Drill and Via Information
- Standard drill size: 0.6 mm for pads
- Via drill size: 0.6 mm
- Via type: Through-hole plated vias
- Annular ring: Minimum 0.15 mm

## Assembly Notes
- Use lead-free solder paste with a reflow profile optimized for the chosen components.
- Stencil thickness: ~0.1 mm stainless steel (adjust as required).
- Verify polarity/orientation of ICs before reflow.

## Testing
- Electrical continuity test after assembly
- Functional test via I2C (SDA/SCL) and power rails (VDD/GND)

## Additional Notes
- Use IPC-2221 as a general PCB design guideline reference (as applicable).
- Confirm footprint dimensions against component datasheets and the actual KiCad sources before fabrication.

---
For corrections, align this document with the authoritative PCB revision and update accordingly.
