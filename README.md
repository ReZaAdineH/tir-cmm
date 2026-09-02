# TIR-CMM — Threat-Informed Response Capability Maturity Model

**You would see it. Could you stop it?**

**Canonical model version: v1.0 · published 24 August 2026**
**8 domains · 58 sub-capabilities · 8×8 Containment Lattice · 7 constraint families / 8 enforced checks**
**Canonical website: https://tir-cmm.com**

TIR-CMM is a threat-informed response capability maturity model that measures whether an organisation can act on what it detects **inside the adversary's breakout window, with someone authorised to act, at the intended blast radius — and whether it can prove that capability**.

TIR-CMM is the **response measurement module of UTIOM**, the Unified Threat-Informed Operations Model, and the companion to **TID-CMM**, which measures detection capability.

> **TID-CMM asks: would we see it? TIR-CMM asks: could we stop it?**

TIR-CMM does not replace UTIOM and does not add a new UTIOM lifecycle phase. UTIOM remains the overarching operating model. TIR-CMM adds measurement depth to the response and continuous-improvement capabilities already defined within UTIOM's Operations & Analysis pillar.

## Use the canonical release

- **Learn about the model:** https://tir-cmm.com/what-is-tir-cmm
- **Run an assessment:** https://tir-cmm.com/assessment
- **Download the specification, workbook and integration artifacts:** https://tir-cmm.com/downloads
- **Check versions and compatibility:** https://tir-cmm.com/changelog
- **Read the licence:** https://tir-cmm.com/licence.html

This repository is the public information, documentation and community surface for TIR-CMM. The canonical website remains authoritative for the released model, assessment tool, downloads, schemas and machine-readable artifacts. Production website and assessment-tool source are intentionally outside this repository.

---

## What TIR-CMM measures

The model scores eight domains and 58 sub-capabilities from 0 to 5.

| ID | Domain | Weight | Subs | Core question |
| --- | --- | ---: | ---: | --- |
| **RP** | Response Preparation & Readiness | 10% | 7 | Are we set up to run an incident at all? |
| **RA** | Response Authority & Decision Rights | 12% | 6 | Is someone permitted to act, in time? |
| **RE** | Response Engineering & Playbooks | 16% | 10 | Is response engineered, or written? |
| **CE** | Containment, Eradication & Recovery | 14% | 8 | Do we have graded options that work? |
| **AO** | Automation & Orchestration | 12% | 7 | Does machine speed reach the decision? |
| **FI** | Forensics, Evidence & Investigation | 10% | 6 | Do we know what actually happened? |
| **RV** | Response Validation & Exercising | 14% | 7 | Have we proven any of this? |
| **RG** | Response Governance, Metrics & Improvement | 12% | 7 | Does it improve, and can we report it? |

TIR-CMM deliberately contains **no detection domain**. It consumes detection maturity as an input constraint, preserving the boundary with TID-CMM.

---

## One model, three assessment depths

TIR-CMM v1.0 supports three strict-superset depths:

- **Pulse** — about 20 minutes, 20 questions, indicative, band capped at L3.
- **Baseline** — about 1–2 hours, all 58 sub-capabilities plus evidence levels, Containment Lattice, authority map and response tempo, band capped at L4.
- **Assurance** — about 2–4 weeks, adds telemetry attributes, exercised scenarios and governance/independent challenge; no ceiling from assessment depth.

The depth reached is itself evidence about how far the result can be trusted.

---

## The Containment Lattice

The atomic unit of TIR-CMM response coverage is an **8×8 Containment Lattice**: eight attack-path stages crossed with eight asset classes.

The first stage is **S0 Prevent & Harden**, because prevention buys the one resource response cannot manufacture: time.

Each in-scope cell is scored from 0 to 3. The lattice is scoped by crown jewels and modelled attack paths rather than treated as a generic 64-cell checklist.

TIR-CMM reports the gap between:

- **Engineered rate** — where the organisation believes it can act; and
- **Proven rate** — where it has shown it can act through exercise or validation.

---

## Two headline metrics

### Validated Response Score (VRS)

The response analogue of TID-CMM's Validated Coverage Score. It is computed across in-scope Containment Lattice cells and reports engineered versus proven response coverage.

### Containment Margin

Response maturity is a race against the adversary:

`Containment Margin = Breakout Time − (MTTD + MTTDecide + MTTC)`

Where:

- **MTTD** = mean time to detect;
- **MTTDecide** = mean time from validated alert to authorised containment decision;
- **MTTC** = mean time to execute containment after authorisation.

TIR-CMM treats **MTTDecide** as a first-class metric because decision latency is often the most fixable but least visible response bottleneck.

In v1.0, tempo inputs carry a source and date. Estimated breakout or interval timings may support planning, but they cannot evidence a validated capability and therefore cap the reported band at L3.

---

## Seven constraint families, eight enforced checks

TIR-CMM retains the seven numbered families R1–R7. Version 1.0 enforces R5b separately in the machine-readable model, so implementations expose eight checks. Every check can only lower a claim.

| ID | Constraint | Core rule |
| --- | --- | --- |
| **R1** | Rehearsal Ceiling | An unrehearsed capability cannot outrank the Response Validation domain by more than one level. |
| **R2** | Authority Ceiling | Automation and containment cannot outrun the authority to use them. |
| **R3** | Evidence Cap | Evidence level VC0–VC3 caps the score a claim can support. |
| **R4** | Detection Dependency | Response Engineering, Containment and Forensics cannot outrun detection maturity. |
| **R5** | Tempo Ceiling | A capability slower than adversary breakout time cannot claim high maturity. |
| **R5b** | Tempo Evidence Ceiling | Estimated breakout or interval timings cap the reported band at L3. |
| **R6** | Blind-Cell Gate | A critical crown-jewel path with no response option caps the reported band. |
| **R7** | Assessment Depth & Governance | Pulse/Baseline depth and insufficient independent challenge cap the reported band. |

See [`docs/04-scoring-and-constraints.md`](docs/04-scoring-and-constraints.md).

---

## Where it sits in UTIOM

UTIOM remains the foundation:

**Vision → Strategy → Crown Jewels → Threat Visibility → Threat Detection → Response → Continuous Improvement**

- **TID-CMM** adds measurement depth within **Engineering & Enablement**: “Would we see it?”
- **TIR-CMM** adds measurement depth within **Operations & Analysis**: “Could we stop it?”

The modules do not fill gaps in UTIOM. They deepen measurement of capabilities UTIOM already defines.

RSMM supports the same Engineering & Enablement pillar by measuring the SIEM and monitoring platform underneath detection operations. It does not change TIR-CMM's scope.

---

## Public knowledge base

Start at [`docs/README.md`](docs/README.md). The repository documents the published model, assessment depths, Containment Lattice, scoring, seven constraints, response tempo, evidence classes, standards alignment, relationship to UTIOM/TID-CMM, limitations and open design questions.

For AI/search discovery, see [`llms.txt`](llms.txt).

---

## Community and challenge

TIR-CMM v1.0 is published for practitioner validation. The most valuable contribution is a counter-example:

- a constraint that fired incorrectly;
- a lattice cell that cannot be scored honestly;
- an asset class or attack-path stage the lattice cannot express;
- measured MTTDecide data;
- an engineered-versus-proven gap that contradicts the model's expectations;
- evidence about any published open design question.

Read [`COMMUNITY.md`](COMMUNITY.md), [`CONTRIBUTING.md`](CONTRIBUTING.md) and [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md).

Security findings must be reported privately under [`SECURITY.md`](SECURITY.md).

---

## Licensing boundary

The repository follows the canonical site's published licensing split:

- **TIR-CMM model** — CC BY-ND 4.0. Use, share, quote and publish results with attribution; derivative models are not permitted under that licence.
- **Schemas and machine-readable model/integration contracts** — CC BY 4.0.
- **Tooling/site/reference implementation** — source-available, all rights reserved; free to run, self-host and audit, but not to redistribute as your own product.

This repository is the public framework/community surface. It does not automatically publish the assessment-tool source or private implementation material.

Canonical licence terms: https://tir-cmm.com/licence.html

---

## Framework family

- **UTIOM — Unified Threat-Informed Operations Model** — https://utiom.de
- **TID-CMM — detection capability depth** — https://tid-cmm.com
- **TIR-CMM — response capability depth** — https://tir-cmm.com
- **RSMM — Realistic SIEM Maturity Model** — https://rsmm.rezaadineh.com/
- **KEVMAP** — https://kevmap.io

Created by **Reza Adineh**.  
https://rezaadineh.com

**Think smarter, Stay Secure.**
