# Contributing to TIR-CMM

TIR-CMM is published for challenge. A useful contribution is evidence that the model, constraint, lattice or timing assumption behaves differently in a real environment than the specification predicts.

Canonical site: https://tir-cmm.com

## What is most useful

### Constraint counter-examples

Identify the exact constraint, the scores/timing/evidence that caused it to fire, and why the resulting ceiling was obviously too strict or too lenient.

### Containment Lattice problems

Describe a cell that cannot be scored honestly on the published 0–3 scale, an asset class the lattice cannot represent, or an attack-path stage that does not fit the response reality of your environment.

### Response tempo evidence

Measured MTTDecide, MTTC, breakout-time assumptions and Containment Margin examples are especially useful. Remove incident-sensitive and organisation-identifying details unless publication is authorised.

### Standalone-route calibration

If you used TIR-CMM without a TID-CMM import, comparisons between the built-in prerequisite score and a later TID-CMM assessment are highly valuable for calibrating R4 and the assessment ceiling.

### Standards and implementation evidence

Crosswalk corrections, OT/ICS examples, cloud/SaaS response cases, exercise results and implementation stories are welcome.

## Change rules

- Scoring changes must be explicit and versioned.
- Constraint changes require numerical reasoning or real counter-evidence.
- The 8-domain response scope must remain distinct from TID-CMM's detection scope unless the canonical model itself is deliberately revised.
- UTIOM remains the operating-model foundation.
- Product procurement must not become a maturity requirement.
- Changes that alter score comparability belong in the changelog.

## Community channels

Use Discussions for interpretation, research, implementation stories and early ideas. Use Issues for actionable defects and model-change proposals. See `COMMUNITY.md` and `CODE_OF_CONDUCT.md`.

## Security

Do not report vulnerabilities publicly. Follow `SECURITY.md`.
