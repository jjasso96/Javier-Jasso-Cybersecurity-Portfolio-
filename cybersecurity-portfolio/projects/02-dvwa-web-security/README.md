# Project 2: DVWA Web Application Security Lab

**Project type:** Hands-on web application security learning  
**Application:** Damn Vulnerable Web Application (DVWA)  
**Environment:** Personal cybersecurity lab using UTM  
**Status:** Application access, login, and security-settings familiarization completed; structured testing and evidence collection remain pending

## Overview

Damn Vulnerable Web Application (DVWA) is an intentionally vulnerable application designed for security education and controlled testing.

During this project, I accessed DVWA, logged in, navigated the interface, and opened its security settings. The next stage is to perform structured tests in the authorized lab and document the actual observations.

Accessing the application does not by itself confirm a vulnerability or demonstrate successful exploitation.

## Objectives

- Become familiar with the DVWA interface and security settings.
- Learn a repeatable approach to controlled web application testing.
- Record procedures and observed application behavior.
- Explain security implications only when supported by test evidence.
- Connect verified observations to appropriate remediation guidance.

## Environment and Tools

| Component | Role |
|---|---|
| DVWA | Intentionally vulnerable web application |
| Kali Linux | Cybersecurity learning environment |
| Web browser | Application access and interaction |
| UTM | Virtualization platform used in the home lab |

The VM networking mode and isolation configuration have not been verified from retained settings.

## Work Completed

- Accessed the DVWA web interface.
- Logged into the application.
- Navigated the interface.
- Accessed the application's security settings.

The exact security level selected and supporting screenshots are not currently retained in this report.

## Testing Status

No individual vulnerability tests, confirmed findings, or remediation results are documented here as completed.

The following are **proposed test areas**, not a record of completed tests:

| Test area | Learning objective |
|---|---|
| SQL injection | Understand how unsafe query construction can expose or alter data |
| Cross-site scripting (XSS) | Examine how untrusted input may be interpreted by a browser |
| Command injection | Understand risks from passing untrusted input to operating system commands |
| File upload security | Examine file validation and upload controls |
| Authentication and session management | Explore relevant authentication and session behaviors |

Any tests should remain within the authorized lab scope.

## Methodology for Future Tests

For each test, record:

1. **Objective:** The behavior being evaluated.
2. **Conditions:** The DVWA security level and relevant configuration, once verified.
3. **Procedure:** The steps actually performed.
4. **Observation:** The application response, captured accurately.
5. **Analysis:** What the observation does and does not demonstrate.
6. **Remediation:** Relevant defensive controls, where applicable.
7. **Evidence:** Sanitized screenshots or reproducible supporting records.

## Security Considerations

- Keep DVWA within a controlled, authorized lab.
- Verify networking and isolation before conducting additional tests.
- Do not expose DVWA to the public internet.
- Remove credentials, session cookies, and sensitive details from published evidence.
- Do not report a vulnerability as confirmed without supporting results.

## Skills Practiced

- Web application navigation
- Application security-settings familiarization
- Controlled testing methodology planning
- Evidence-based technical documentation
- Risk awareness and remediation analysis

## Next Steps

- [ ] Record the selected DVWA security level after verifying it.
- [ ] Capture sanitized screenshots of the application and settings.
- [ ] Select one initial test case and document its objective.
- [ ] Perform the test within the authorized lab.
- [ ] Record the actual result and supporting evidence.
- [ ] Explain the security implications and relevant remediation.
- [ ] Update the project status to reflect completed work.

## Evidence

**Current evidence status:** No supporting screenshots or exported test results are currently retained for this report.

Future evidence should be added only after the test is performed and observations are verified.

**Current outcome:** DVWA access and interface familiarization completed. Structured security testing, finding validation, and remediation documentation remain outstanding.
