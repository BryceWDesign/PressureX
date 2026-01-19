# PressureX (Pressure X)

**Passive structural mitigation layer — evaluation package (design-intent, not validated flight hardware).**

PressureX is a **narrowly-scoped, passive** structural sub-layer concept intended to **reduce peak transmitted acceleration** and **broaden impulsive load duration** in aerospace structures via controlled compliance + dissipation. It is designed to be **testable, falsifiable, and integrable** within existing architectures—without exotic physics or mission-critical dependence.

## What this repo is
- An **engineering evaluation package** for a passive mitigation layer: scope, targets, limits, baselines, and a staged validation plan.
- A small **conceptual simulation** (illustrative only) to support early parameter intuition and discussion.

## What this repo is not
PressureX is **not**:
- A primary load-bearing structure
- A replacement for pressure vessels / hull skins
- A Whipple shield or MMOD penetration-prevention system
- An active control system, power system, or “smart structure” requiring electronics

See **SYSTEM_BOUNDARIES.md** for explicit inclusions/exclusions.

## Status (read this first)
- **Design-intent only:** performance values are **targets/hypotheses**, not achieved results.
- **No qualification claim:** any included test protocols/logs are provided for evaluation workflow; they are **not evidence of completed qualification** unless accompanied by traceable raw data + setup details.

## Quick review map (engineer-first)
Start here:
- **SYSTEM_BOUNDARIES.md** — scope, classification, non-capabilities
- **ENGINEERING_README_APPENDIX.md** — 1-page technical summary + open questions
- **PERFORMANCE_TARGETS.md** — design-intent targets (explicitly not results)
- **COMPARATIVE_BASELINE.md** — what “good” must beat, and where it fits
- **FAILURE_MODES_AND_LIMITS.md** — failure thinking up front
- **VALIDATION_PATH.md** — staged validation + explicit kill criteria

## Conceptual simulation (illustrative, not validation)
A minimal model exists to demonstrate parameter sensitivity and produce an output plot:
- `src/stararmor_simulation.py`
- Outputs saved under `outputs/`

To run:
1. Install Python deps: `pip install -r requirements.txt`
2. Run: `python src/stararmor_simulation.py`

**Note:** This script is a **conceptual model** and must not be treated as proof of structural performance.

## Optional instrumentation / test artifacts (separate from the passive layer)
This repo also contains **prototype instrumentation and test documentation** under:
- `PressureX/` (sensor/PCB/mechanical/test-protocol artifacts)

These items are intended as **optional validation tooling** and do not change the passive nature of the mitigation layer concept. They should be treated as **prototype-grade** unless explicitly backed by traceable data.

## License
Licensed under **IX-PressureX Open Technology License (IX-PressureX-OTL)** — see `LICENSE`.  
Civilian / industrial / research / educational use only; military/weaponized use is prohibited.

## Contact / Technical review
If you work in **structures / dynamics / test** and want to evaluate quickly, the repo is structured to support a fast “prove or kill” review. The most useful feedback is: *which single test would falsify this fastest, and what pass/fail metric would you use?*
