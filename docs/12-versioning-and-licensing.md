# TIR-CMM Versioning and Licensing

## Canonical version history

The TIR-CMM changelog explicitly states:

- **v0.1 — 16 August 2026**: first complete model; 8 domains, 58 sub-capabilities, a 7-stage × 8-asset lattice and five integrity constraints.
- **v0.2 — 17 August 2026**: three assessment depths, graduated evidence ceilings, S0 Prevent & Harden, standalone prerequisite route, R7, exclusion of unscored domains, timing validation and other scoring corrections.
- **v1.0 — 24 August 2026**: first stable release; enforced proof recency, sourced tempo evidence and R5b, normative interval definitions, complete export metadata, advisory consistency checks, resolved R4 basis and corrected standards crosswalks.

The current canonical model is **v1.0**. The browser tool/library is **v1.0.0**, the export schema is **v1.0**, and the workbook is **v1.0**. These versions are independent by design and must be recorded separately in exported assessment results.

Version authority and compatibility rules: https://tir-cmm.com/changelog

## Licensing boundary

The canonical site publishes a split licence:

### Model — CC BY-ND 4.0

The conceptual TIR-CMM model may be used, shared, quoted and used commercially with attribution, but derivative models are not permitted under the published licence. The purpose is to preserve score comparability: a TIR-CMM score should refer to one model rather than incompatible forks using the same name.

### Schemas and machine-readable model — CC BY 4.0

Published schemas and machine-readable integration contracts can be used for integrations, including commercial integrations, with attribution.

### Tooling/site/reference implementation — source-available, all rights reserved

The published tooling is described as free to run, self-host and audit, but not licensed to be redistributed or rebranded as another product.

This GitHub repository therefore focuses on the public framework, documentation, community and intentionally open integration artifacts. It does not assume that all website/tooling source should be made public merely because the tool is free to use.

Canonical licence and changelog: https://tir-cmm.com
