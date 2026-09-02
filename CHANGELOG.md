# TIR-CMM Changelog

This repository follows the explicit version history published by the canonical TIR-CMM website: https://tir-cmm.com.

## [1.0] — 2026-08-24

First stable model release. The eight domains, 58 sub-capabilities, 8×8 Containment Lattice and seven numbered constraint families remain intact, while the evidence, timing and compatibility rules are made operational and reproducible. R5b is represented separately in the machine-readable model, giving implementations eight enforced checks.

Key published changes include:

- R5b caps the reported band at L3 when breakout evidence is neither measured nor actor-specific, or when response intervals are estimated;
- breakout time records its source, reference and date;
- MTTDetect, MTTDecide and MTTContain have normative start and stop events, with P50/P90, sample size, measurement window and data source where available;
- Proven lattice status and VC3 evidence require dates and expire after 12 months, or sooner after a material tooling, on-call, ownership, architecture or provider change;
- all applicable band ceilings are retained and reported, even when another ceiling is already more restrictive;
- 13 advisory consistency checks identify likely scoring errors without changing the score;
- R4 now uses TID-CMM's constraint-adjusted, pre-substitution overall detection score;
- exports carry the complete model, tool, schema and assessment metadata contract;
- blueprint items include impact, effort, horizon, acceptance criteria and closure fields;
- S0 Prevent & Harden has an explicit scope boundary;
- optional ATT&CK, D3FEND, actor and procedure traceability may be recorded beneath lattice cells;
- the OT/ICS profile is published as an explicitly unvalidated extension design;
- standards crosswalk corrections were made against primary sources.

Current artifact versions:

| Artifact | Version |
| --- | --- |
| Model | 1.0 |
| Browser tool and library | 1.0.0 |
| Export schema | 1.0 |
| Workbook | 1.0 |

Migration note: v0.2 progress files load into the v1.0 tool. Undated Proven cells revert to Engineered, undated VC3 evidence grades to VC2, and estimated tempo inputs cap the band at L3 until the required evidence is added.

## [0.2] — 2026-08-17

Second published model iteration.

Key published changes include:

- three assessment depths: Pulse, Baseline and Assurance;
- graduated evidence classes VC0–VC3;
- S0 Prevent & Harden added to the Containment Lattice;
- standalone prerequisite route when TID-CMM is unavailable;
- seventh integrity constraint covering assessment depth and governance;
- corrections to scoring and domain-exclusion behaviour;
- timing validation and stronger response-tempo treatment;
- 8-stage × 8-asset Containment Lattice;
- 7 integrity constraints.

## [0.1] — 2026-08-16

First complete published model:

- 8 response domains;
- 58 sub-capabilities;
- 7-stage × 8-asset containment lattice;
- five initial integrity constraints.
