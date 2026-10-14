# Project 4: Tenable Nessus Vulnerability Assessment

**Status:** In progress / assessment evidence to be added  
**Goal:** Complete and document an end-to-end vulnerability assessment of an authorized lab target.

## Objective

Demonstrate the vulnerability management workflow using Tenable Nessus: define scope, run a scan, interpret findings, prioritize remediation, and validate the results.

## Planned Lab

Previous planning considered using a dedicated Ubuntu Server ARM64 VM and scanning an authorized lab target such as the Kali/DVWA environment. Confirm the final setup before documenting it as implemented.

**Do not expose DVWA or another deliberately vulnerable service to the public internet.** Confirm the VM network configuration and restrict access to the lab.

## Workflow

### 1. Scope and preparation
- Record the target and why it is authorized.
- Record VM operating systems, network mode, and relevant IP information in a sanitized form.
- Confirm Nessus edition/version and target reachability.
- Document any credentials or scan settings without publishing secrets.

### 2. Scan
- Create a suitable scan for the lab target.
- Record the scan policy and relevant settings.
- Run the scan and preserve sanitized evidence.
- Note scan limitations, unreachable services, or incomplete checks.

### 3. Analyze
For selected findings, record:
- Finding/plugin name and ID
- Affected host/service
- CVE, if applicable and verified
- CVSS information and its source
- Scanner evidence and affected version/configuration
- Business/technical impact in the lab context
- Confidence and limitations

### 4. Prioritize and remediate
- Select a finding based on evidence and context.
- Research an appropriate fix using a trustworthy vendor or project source.
- Apply the fix only to the lab target.
- Record the change and any potential service impact.

### 5. Validate
- Re-scan using a comparable configuration.
- Compare the original and follow-up evidence.
- State whether the finding was resolved, remains present, or could not be validated.
- Explain any residual risk or limitations.

## Results Table

| Finding | Evidence | Risk rationale | Recommended fix | Status after validation |
|---|---|---|---|---|
| To be populated from scan | Pending | Pending | Pending | Pending |

## Deliverables

- [ ] Lab architecture diagram
- [ ] Sanitized scan configuration/results screenshots
- [ ] Findings table with evidence
- [ ] Prioritized remediation plan
- [ ] Before/after comparison
- [ ] Final report with limitations and lessons learned

## Reporting Integrity

Do not claim a scan was run, a vulnerability was found, or a remediation succeeded until you have the corresponding evidence. Keep any example data clearly labeled as synthetic.
