# TIR-CMM Scoring and Seven Integrity Constraints

Every sub-capability is scored from 0 to 5. Domain scores are weighted means of in-scope sub-capabilities; the overall score is the weighted mean of the eight domain scores.

The Containment Lattice is reported alongside maturity rather than folded into the arithmetic, but it can still bind the reported band through R6.

## Application order

The published scoring order is:

1. R3 — Evidence Cap at sub-capability level
2. Compute domain scores
3. R4 — Detection Dependency
4. R2 — Authority Ceiling
5. R1 — Rehearsal Ceiling
6. Compute overall score
7. Apply R5, R6 and R7 to the reported band; the lowest cap wins

Constraints can only lower a claim.

## R1 — Rehearsal Ceiling

All domains except Response Validation are capped at **RV + 1**. An unrehearsed playbook remains an assumed capability.

## R2 — Authority Ceiling

Automation & Orchestration and Containment/Eradication/Recovery are capped at **Response Authority + 1**. Automation that nobody is authorised to execute is not operational capability.

## R3 — Evidence Cap

Version 0.2 uses graduated evidence levels:

| Evidence | Name | Score ceiling |
| --- | --- | ---: |
| VC0 | Assertion only | 1 |
| VC1 | Design or policy | 2 |
| VC2 | Implemented and tested | 4 |
| VC3 | Repeatably validated | 5 |

The evidence level is a ceiling, not a conversion; strong evidence does not increase a low capability score.

## R4 — Detection Dependency

Response Engineering, Containment and Forensics cannot exceed detection maturity + 1. TIR-CMM uses an imported TID-CMM score where available or a clearly flagged standalone proxy.

## R5 — Tempo Ceiling

The reported band is constrained by whether containment arrives before adversary breakout. A response capability structurally slower than the adversary cannot claim high maturity regardless of documentation quality.

## R6 — Blind-Cell Gate

A Tier-1 crown-jewel lattice cell with no response option caps the band at L2.

## R7 — Assessment Depth & Governance Ceiling

Pulse caps the band at L3. Baseline caps it at L4. A result without evidence-led scoring, independent calibration and separation of assessor from approver is also capped at L4.

Canonical scoring page: https://tir-cmm.com/scoring