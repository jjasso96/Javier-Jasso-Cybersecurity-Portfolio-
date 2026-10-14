# Project 2: DVWA Web Application Security Lab

**Project type:** Hands-on web application security learning  
**Status:** Application access verified; security testing and evidence collection pending  
**Application:** Damn Vulnerable Web Application (DVWA)  
**Environment:** Personal cybersecurity lab

## Overview

This project uses Damn Vulnerable Web Application (DVWA), an intentionally vulnerable web application designed for security education and controlled testing.

I configured the lab environment, accessed the DVWA interface, logged in, and explored its security settings. The next phase is to conduct structured tests against selected application features, document observations, and identify appropriate remediation measures.

The goal is to develop practical skills in web application security, vulnerability validation, and evidence-based technical reporting.

## Objectives

- Become familiar with the DVWA interface and security configuration.
- Understand common web application vulnerability classes.
- Practice controlled security testing in an authorized environment.
- Document test procedures, observations, and potential security implications.
- Connect technical findings to remediation recommendations and vulnerability management practices.

## Environment and Tools

| Component | Purpose |
|---|---|
| DVWA | Intentionally vulnerable web application |
| Kali Linux | Cybersecurity learning environment |
| Web browser | Application access and interaction |
| UTM | Virtualization platform used in the home lab |

The exact VM networking mode and network isolation configuration have not yet been verified.

## Work Completed

### Application Access

- Successfully accessed the DVWA web interface.
- Logged into the application.
- Navigated the application interface.
- Accessed the security settings.

### Current Testing Status

No individual vulnerability tests, confirmed findings, or remediation results have been documented in this report yet.

Accessing DVWA establishes that the application is reachable; it does not establish that a vulnerability has been successfully tested or exploited.

## Planned Security Assessment

The following are proposed test areas, not completed tests or confirmed findings.

| Test area | Assessment goal |
|---|---|
| SQL injection | Understand how unsafe database query handling can expose application data |
| Cross-site scripting (XSS) | Examine how untrusted input may be interpreted as browser-executable content |
| Command injection | Understand the risks of passing untrusted input to operating system commands |
| File upload security | Examine file validation and upload handling controls |
| Authentication and session management | Evaluate relevant authentication and session security behaviors |

Testing will be conducted only against the authorized lab application.

## Methodology

For each test, the assessment record will include:

1. **Objective:** What behavior or vulnerability is being evaluated.
2. **Configuration:** The DVWA security level and relevant test conditions.
3. **Procedure:** The steps performed to reproduce the test.
4. **Observation:** The actual application response.
5. **Analysis:** What the result does and does not demonstrate.
6. **Remediation:** Recommended security controls, where applicable.
7. **Evidence:** Sanitized screenshots or other reproducible supporting records.

## Security Considerations

- Keep DVWA within a controlled, authorized lab environment.
- Verify network configuration before conducting additional tests.
- Do not expose DVWA to the public internet.
- Remove credentials, session cookies, and sensitive information from published evidence.
- Do not report a vulnerability as confirmed without supporting test results.

## Skills Developed

- Web application navigation and configuration
- Security testing methodology
- Vulnerability validation
- Technical documentation
- Risk awareness and remediation analysis
- Evidence-based reporting

## Next Steps

- [ ] Record the selected DVWA security level.
- [ ] Capture sanitized screenshots of the application and settings.
- [ ] Select an initial test case and document its objective.
- [ ] Perform the test in the authorized lab.
- [ ] Record the actual result and supporting evidence.
- [ ] Explain the security implications and potential remediation.
- [ ] Update the project status as testing progresses.

## Evidence

**Current evidence status:** No supporting screenshots or exported test results have been collected for this report.

Evidence will be added as testing is performed and observations are verified.

**Project outcome:** DVWA access and interface familiarization completed. Structured security testing, findings validation, and remediation documentation remain future work.
