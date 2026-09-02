# Response Tempo, MTTDecide and Containment Margin

TIR-CMM treats response maturity as a race against the adversary.

## Containment Margin

For each priority actor:

`Containment Margin = Breakout Time − (MTTD + MTTDecide + MTTC)`

Where:

- **Breakout Time** is the time from initial foothold to first lateral movement;
- **MTTD** is mean time from initial foothold to validation as a real incident;
- **MTTDecide** is mean time from validated alert to authorised containment decision;
- **MTTC** is mean time from authorisation until containment has taken effect.

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

## Evidence quality in v1.0

Breakout time records a source, reference and date. The source hierarchy is:

1. observed in the organisation's own incidents or exercises;
2. actor-specific threat intelligence;
3. sector-specific evidence;
4. a published industry benchmark;
5. an assessor estimate.

The first two qualify as measured for the tempo constraint. The remaining sources are estimates for the assessed environment and cap the reported band at L3 under R5b. Where available, each interval should also record P50, P90, sample size, measurement window and data source; a mean based on fewer than ten timed incidents is flagged as underpowered.

Canonical site: https://tir-cmm.com
