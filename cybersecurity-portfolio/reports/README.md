# Security Assessment Reports and Evidence

## Purpose

This directory organizes supporting documentation for cybersecurity projects, including assessment reports, technical observations, remediation recommendations, and sanitized evidence.

The goal is to make work traceable and understandable while distinguishing verified observations from planned activities, general learning, and unvalidated scanner output.

## Minimum Reporting Standard

Where applicable, each report should document:

- **Objective:** What the activity was intended to evaluate.
- **Scope and authorization:** The permitted target and assessment boundaries.
- **Environment:** Relevant systems, tools, and configurations that were actually used.
- **Method:** The procedures performed.
- **Observations and findings:** Results supported by evidence.
- **Analysis:** What the evidence supports and what remains uncertain.
- **Risk context:** Severity, exposure, impact, and business relevance when known.
- **Recommendations:** Appropriate corrective actions, where justified.
- **Validation:** Evidence that a corrective action worked, if remediation and verification were performed.
- **Limitations:** Missing artifacts, constraints, and unanswered questions.

Do not fill missing details with assumptions. Use “not recorded” or “not verified” when appropriate.

## Evidence Handling

Useful evidence may include:

- Sanitized screenshots of tool configuration and results.
- Exported vulnerability assessment reports.
- Relevant commands and output.
- Vulnerability identifiers and authoritative technical references.
- Reproduction notes, remediation records, and validation results.

Before publication, remove credentials, tokens, personal information, sensitive network details, private target information, and confidential employer data. Check screenshots for browser tabs, usernames, session cookies, IP addresses, MAC addresses, SSH host-key fingerprints, password lists, and other accidental disclosures. Do not commit raw screenshots merely because they are useful; create a sanitized copy first or document the observation without publishing the image.

## Current Project Documentation

| Project | Current documented scope |
|---|---|
| [Project 1: Home Cybersecurity Lab](../projects/01-home-cybersecurity-lab/README.md) | Linux VM connectivity, ping, Nmap service discovery, SSH access, and a UFW rule update; firewall enforcement and isolation remain unverified |
| [Project 2: DVWA Web Security](../projects/02-dvwa-web-security/README.md) | Hydra HTTP-form exercise; tool-reported successes conflict with the browser's login-error/lockout message and remain unverified |
| [Project 3: Vulnerability Management](../projects/03-vulnerability-management/README.md) | Learning and workflow documentation; no specific findings claimed without evidence |
| [Project 4: Nessus Assessment](../projects/04-nessus-assessment/README.md) | TryHackMe scan completed and results reviewed; original artifacts unavailable |

Project 1 and Project 2 have been updated from screenshots reviewed during this documentation pass. The original images are not included in the repository because they expose host/account details. The written summaries omit exact lab addresses, usernames, password candidates, MAC addresses, and SSH fingerprints.

The reports describe only the work and results supported by available evidence. Missing scan statistics, specific findings, and remediation outcomes must not be inferred.

## Suggested Evidence Naming

Use descriptive, non-sensitive filenames, for example:

- `project-01-utm-vm-settings-sanitized.png`
- `project-01-network-scan-sanitized.png`
- `project-02-dvwa-brute-force-sanitized.png`
- `project-04-nessus-results-sanitized.png`

These are naming examples only, not files that currently exist. Never include credentials or sensitive target information in filenames.

## Before Publishing a Report

- [ ] Confirm the activity was completed and authorized.
- [ ] Separate direct observations from interpretation.
- [ ] Check that all numbers, identifiers, and claims match the source evidence.
- [ ] Label planned tests as planned rather than completed.
- [ ] Do not claim a vulnerability is confirmed based only on unvalidated scanner output.
- [ ] Do not claim remediation or risk reduction without validation.
- [ ] Sanitize screenshots and exports.
- [ ] Remove passwords, tokens, cookies, private keys, IP addresses when unnecessary, MAC addresses, and host-key fingerprints.
- [ ] Link the report to its corresponding project README.

## Professional Practice

Tool familiarity, completed scans, scanner-reported findings, manually validated vulnerabilities, and verified remediation are different outcomes. Document each at the level supported by the evidence.
