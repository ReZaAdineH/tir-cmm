# Evidence and Response Validation

TIR-CMM separates claimed capability from demonstrated capability.

Version 0.2 replaces a yes/no evidence flag with four evidence classes:

- **VC0 — Assertion only**: verbal claim or no evidence; caps at 1.
- **VC1 — Design or policy**: document, policy, screenshot or partial implementation; caps at 2.
- **VC2 — Implemented and tested**: implementation evidence plus a test result, ticket or system record; caps at 4.
- **VC3 — Repeatably validated**: recent, repeatable and independently reviewable proof from the live environment; caps at 5.

Evidence permits a score; it does not create one.

## Response Validation & Exercising

The RV domain exists because response content can remain dormant for months. A playbook can look correct while failing at first execution because tooling changed, privileges expired, a dependency moved, an approval path is unavailable, or the business impact was never accepted.

TIR-CMM therefore values exercises that execute actual response capability under a clock rather than treating discussion-only tabletop activity as equivalent proof.

At Assurance depth, scenario validation adds recorded lifecycle stages, pass conditions, timing and recovery targets. An exercise without observed timing cannot establish response readiness against adversary tempo.

## Engineered versus proven

The Containment Lattice makes the evidence gap visible as two rates:

- Engineered rate — we believe we can act here.
- Proven rate — we have shown we can act here.

The difference between those rates is intentionally treated as a finding rather than averaged away.

Canonical site: https://tir-cmm.com