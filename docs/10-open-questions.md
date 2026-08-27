# TIR-CMM Open Questions and Contribution Priorities

TIR-CMM v0.2 is deliberately published for challenge. The canonical About/changelog material keeps unresolved design questions visible rather than presenting the model as empirically settled.

High-value questions include:

1. **R4 basis** — should detection dependency use TID-CMM overall maturity or a harsher visibility-related basis?
2. **Lattice/domain coupling** — should the Containment Lattice remain reported alongside maturity or become a pseudo-domain?
3. **Standalone calibration** — is the prerequisite-check threshold and L4 ceiling calibrated correctly for organisations without TID-CMM?
4. **OT/ICS depth** — does the OT asset class need dedicated response sub-capabilities because safe-state, manual fallback and reimaging assumptions differ materially from IT?
5. **Breakout-time fallback** — what default is defensible when actor-specific breakout intelligence is unavailable?
6. **MTTDecide instrumentation** — what practical method produces reliable decision-latency timestamps where case tooling does not natively separate validation from authorisation?
7. **R1 dominance** — is the rehearsal ceiling too dominant, and would an alternative preserve honesty while improving diagnostic spread?
8. **Worked-example publication** — publish and maintain practitioner-facing score sheets and lattice evidence so future model changes can be tested numerically.

One earlier v0.2 question — how to support threat modelling and detection maturity when TIR-CMM is run standalone — is documented by the site as resolved through the eight-question prerequisite check.

## What makes useful feedback

The best contribution is an observed counter-example: a constraint firing incorrectly, a lattice cell that cannot be scored honestly, measured timing that contradicts the model's assumptions, or an environment the published asset/stage structure cannot express.

Canonical open-question source: https://tir-cmm.com/about