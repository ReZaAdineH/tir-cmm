# TIR-CMM Security Policy and Vulnerability Reporting

TIR-CMM includes a public framework repository and a browser-based assessment tool. Security findings should be reported privately.

## Report privately

**Do not publish a suspected vulnerability, exploit, credential, sensitive endpoint, assessment export, incident evidence, or reproduction containing sensitive data in a public Issue or Discussion.**

Preferred reporting paths:

1. If GitHub displays **Report a vulnerability** in this repository's Security area, use that private channel.
2. Otherwise use the contact/security guidance on the canonical site: https://tir-cmm.com.

## In scope

Examples include:

- vulnerabilities in the assessment tool or canonical website;
- unintended transmission or remote storage of assessment data contrary to the browser-local design;
- cross-site scripting, injection, unsafe file import/export, or similar web vulnerabilities;
- exposure of credentials, tokens, private keys, non-public endpoints or private implementation details;
- integrity weaknesses in downloadable models, schemas or assessment artifacts;
- parsing weaknesses in public import/export contracts;
- repository content that accidentally exposes private operational or incident material.

## Public Issues are appropriate for

- model or constraint defects that are not security vulnerabilities;
- lattice/scoring questions;
- standards-mapping corrections;
- documentation and public-link problems;
- open design questions that contain no sensitive incident data.

## Safe-testing boundaries

Do not access data that is not yours, perform denial-of-service or resource-exhaustion testing, use social engineering, establish persistence, move laterally, or run broad automated scanning that could degrade the service.

If sensitive data is encountered, stop, retain only the minimum evidence required for the report, and report privately.

## Coordinated disclosure

Please allow a reasonable period for investigation and remediation before public disclosure. There is currently no bug-bounty promise associated with vulnerability reports.

## Public/private boundary

The public model/community repository does not imply that the assessment tool, site source, production infrastructure, credentials or proprietary/private implementation material are open source. Follow the licensing boundary documented by the canonical site and this repository.