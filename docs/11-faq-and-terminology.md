# TIR-CMM FAQ and Terminology

## What does TIR-CMM stand for?

**Threat-Informed Response Capability Maturity Model.**

## What question does it answer?

**Could we actually stop the attack, in time, with authority, and prove it?**

## Does TIR-CMM measure the incident response team?

Not by itself. It measures the organisation's capacity to act. The binding constraint may sit with business authority, identity/platform ownership, tooling access, legal/regulatory process, recovery capability or other functions outside the formal IR team.

## What is the Containment Lattice?

An 8×8 matrix of attack-path stages and asset classes used to determine where response options exist, are engineered, are proven, or are absent. It is scoped by crown jewels and attack paths.

## What is the Validated Response Score?

A lattice-based response coverage metric showing how much in-scope response capability is engineered and how much has actually been proven.

## What is Containment Margin?

The signed time margin between adversary breakout time and the organisation's total detect-decide-contain time.

## What is MTTDecide?

Mean time from validated alert to an authorised decision to contain. TIR-CMM separates it from execution time because waiting for authority is frequently the true response bottleneck.

## Is TIR-CMM a certification?

No official certification scheme is defined by the published model. Assessment depth and governance determine how strongly the result can be defended.

## Can TIR-CMM run without TID-CMM?

Yes. It can run standalone using a short prerequisite check. A TID-CMM import provides stronger evidence for the detection-dependency constraint and can lift ceilings that apply to an unaudited proxy.

## Does TIR-CMM replace UTIOM?

No. UTIOM is the operating model. TIR-CMM is a deeper response measurement instrument for capabilities UTIOM already defines.

## Evidence classes

- VC0 — Assertion only
- VC1 — Design or policy
- VC2 — Implemented and tested
- VC3 — Repeatably validated

Canonical site and glossary: https://tir-cmm.com