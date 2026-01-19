# Connector Assembly (CAD Placeholder)

> **Status:** Placeholder notes. This repository does **not** currently include an exported STEP model for this part.

The text below captures the intended connector assembly concept so a reviewer can understand the interface assumptions.

## Description
- Connector housing concept with locking interface for external cable
- Mounts to rear of the pressure sensor housing concept
- Integrated strain relief chamber
- Supports ribbon cable or twisted pair (shielded)

## Dimensions (concept)
- Outer dimensions: 15 mm (W) x 12 mm (H) x 20 mm (L)
- Mounting flange: 20 mm x 15 mm
- Cable channel: 6 mm (W) x 4 mm (H)
- Panel slot depth: 3 mm

## Materials (examples)
- Main body: Aluminum 6061 (finish per environment)
- Strain relief insert: Silicone rubber
- Cable clamp: Polycarbonate (or equivalent)

## Features
- Rear-threaded barrel for cable tension fitting
- Optional EMI gasket groove (if required)
- Cable guide rail + tie-down cavity

## Assembly overview
1. Connector seats into housing cutout
2. Cable routes from internal PCB to external port
3. Strain relief seats against internal rib
4. Optional sealant depending on environment
5. Mount with M2 bolts into housing tabs

## To create a real CAD export
Model the geometry in CAD and export the actual STEP file as:
- `connector_assembly.step`

Then remove/replace this placeholder.
