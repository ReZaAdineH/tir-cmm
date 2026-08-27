# Response Tempo, MTTDecide and Containment Margin

TIR-CMM treats response maturity as a race against the adversary.

## Containment Margin

For each priority actor:

`Containment Margin = Breakout Time − (MTTD + MTTDecide + MTTC)`

Where:

- **Breakout Time** is the time from initial foothold to first lateral movement;
- **MTTD** is mean time to detect;
- **MTTDecide** is mean time from validated alert to authorised containment decision;
- **MTTC** is mean time to execute containment once authorised.

A positive margin means containment lands before breakout. A negative margin means the organisation is structurally behind the adversary even if its playbooks and tooling look mature.

## MTTDecide

TIR-CMM makes decision latency visible as its own metric. Conventional MTTR often hides the time spent waiting for approval, risk acceptance, business-owner input or an authorised person to become available.

That separation matters because decision latency is frequently more improvable than technical execution latency.

## Tempo Ratio

The model also reports:

`Tempo Ratio = (MTTD + MTTDecide + MTTC) / Breakout Time`

Interpretation published by the model:

- **TR < 0.5** — meaningful tempo advantage;
- **0.5 ≤ TR < 1.0** — contains before spread with limited margin;
- **1.0 ≤ TR < 2.0** — structurally behind;
- **TR ≥ 2.0** — response is effectively post-incident recovery.

Tempo Ratio drives constraint R5.

Canonical site: https://tir-cmm.com