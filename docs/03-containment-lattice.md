# The TIR-CMM Containment Lattice

The Containment Lattice is the atomic response-coverage structure in TIR-CMM.

It crosses **eight attack-path stages** with **eight asset classes**, producing a 64-cell matrix before scoping. Crown jewels and modelled attack paths reduce that to the working set that actually matters for the organisation, commonly a much smaller subset.

Each in-scope cell is scored from **0 to 3**:

- **0 — no usable response option**;
- **1 — response option exists in principle or procedure**;
- **2 — engineered/implemented response option**;
- **3 — proven through recent exercise or validation**.

Status 3 is not permanent. Proven capability can expire when evidence becomes stale.

## S0 Prevent & Harden

Version 0.2 adds **S0 Prevent & Harden** ahead of the response stages, with the highest stage leverage in the model. The principle is simple: an attack path that architecture prevents never needs a response, and prevention creates the one resource incident response cannot manufacture after compromise — time.

## Why the lattice is separate from domain maturity

The lattice is reported alongside the maturity score rather than folded into it. This prevents broad but shallow response coverage from hiding a structural inability to act on a critical path.

The lattice still affects reported maturity through the Blind-Cell Gate (R6) and through roadmap prioritisation.

## Engineered versus proven

TIR-CMM reports both:

- **Engineered rate** — proportion of in-scope cells at status 2 or above;
- **Proven rate** — proportion at status 3.

The gap between the two is a central finding: what the organisation believes it can do versus what it has actually demonstrated.

Canonical site: https://tir-cmm.com