# Project 2: DVWA Web Application Security Lab

**Project type:** Hands-on web application security learning  
**Application:** Damn Vulnerable Web Application (DVWA)  
**Environment:** Personal virtualized lab using Kali Linux and UTM  
**Status:** DVWA access and a Hydra HTTP-form exercise documented; reported credential results require validation

## Overview

Damn Vulnerable Web Application (DVWA) is an intentionally vulnerable application designed for security education and controlled testing.

Screenshots show the DVWA Brute Force module open in a browser and THC Hydra being used against the lab form with a short list of candidate passwords. Hydra reported six “valid passwords found,” but the visible DVWA page displayed an incorrect-credentials message and warned that the account might be temporarily locked after repeated failed attempts.

Because those results conflict, the tool output is **not treated as proof of valid credentials or a successful login**. The exact target address, account name, candidate passwords, and other host-identifying details are intentionally omitted from this public report.

## Objectives

- Practice controlled authentication testing in an intentionally vulnerable application.
- Learn how automated tool output depends on correctly configured success/failure conditions.
- Compare command-line results with the application’s actual response.
- Document uncertainty rather than presenting unvalidated output as a confirmed finding.
- Identify defensive controls relevant to repeated authentication attempts.

## Environment and Tools

| Component | Role |
|---|---|
| DVWA | Intentionally vulnerable web application |
| Kali Linux | Security testing environment |
| THC Hydra | HTTP form authentication testing tool |
| Web browser | Independent view of the application response |
| UTM | Virtualization platform used for the lab |

The screenshots indicate that the DVWA Brute Force module was open in the browser and that Hydra used an HTTP GET-form workflow. The exact request parameters, target URL, application configuration, and tool invocation are not reproduced because they include unnecessary target-specific details and the original lab notes are not available.

## Work Completed and Observations

- Opened the DVWA Brute Force module.
- Ran a short Hydra HTTP-form test against the lab application.
- Observed Hydra report six candidate passwords as valid.
- Compared the tool output with the browser, where DVWA displayed an incorrect-credentials message and a possible account-lockout warning.

No candidate passwords are reproduced in this report.

## Analysis and Limitations

The conflicting outputs are the most important learning point in this exercise. Automated form-testing tools typically decide whether an attempt succeeded by matching a configured response condition. If the condition is too broad or does not distinguish the successful-login response from a failed-login or lockout response, the tool can report false positives.

The screenshots alone do not establish which response condition Hydra used, whether any candidate credential was actually accepted, or whether a successful authenticated session was reached. Accordingly:

- The six tool-reported results are treated as **unverified candidates**, not confirmed passwords.
- No successful authentication is claimed.
- No confirmed vulnerability severity or exploitability rating is assigned.
- The visible lockout message is documented as an application response, not proof of a specific lockout implementation or duration.
- No remediation or retest is claimed as completed.

## Recommended Validation Workflow

For a future authorized lab run:

1. Confirm the target is the local/authorized DVWA instance and record the relevant module and security level.
2. Use a small, controlled test list and avoid unnecessary repeated attempts.
3. Establish the expected failure response and successful-login response manually before configuring automated detection.
4. Configure the tool’s failure condition to distinguish a failed attempt from a genuinely successful authentication.
5. Validate any reported success by checking the application state in the browser or another reliable independent indicator.
6. Stop if an account-lockout or rate-limit response appears, and document it without assuming the cause.
7. Save sanitized evidence of the request configuration and both failure/success response behavior, if a success can be reproduced.
8. Report only results supported by the validation evidence.

This workflow is guidance for future testing; it does not imply these validation steps were completed during the captured exercise.

## Security Considerations and Defensive Context

Authentication defenses commonly include rate limiting, progressive delays, multi-factor authentication where appropriate, monitoring for repeated failures, and carefully designed account-lockout controls. Lockout policies should also be evaluated for denial-of-service and account-enumeration side effects.

Testing must remain within an authorized lab. Do not use password lists against third-party systems or accounts. Do not publish candidate passwords, session cookies, credentials, private target details, or unredacted screenshots.

## Skills Practiced

- DVWA navigation and authentication-module familiarization
- Hydra HTTP-form testing in a controlled lab
- Comparing automated tool output with browser-observed behavior
- Recognizing false-positive risks in automated testing
- Evidence validation and cautious technical reporting
- Understanding defensive controls for repeated authentication attempts

## Next Steps

- [ ] Recreate the exercise only within the authorized lab.
- [ ] Verify the configured success/failure match condition using known, controlled test cases.
- [ ] Confirm any reported success independently before documenting it as a finding.
- [ ] Record the application’s actual security level and relevant configuration.
- [ ] Capture sanitized evidence without target addresses, account names, candidate passwords, cookies, or tokens.
- [ ] Document defensive recommendations and perform a retest only if changes are actually made.

## Evidence

**Evidence reviewed:** User-provided screenshots of the DVWA Brute Force page and Hydra output.

**Publication status:** Raw screenshots are not included in the public repository because they contain target and account-related details. Candidate passwords and host identifiers have been excluded.

**Current outcome:** The automated tool reported candidate successes, but the browser displayed an authentication failure/lockout message. The result remains inconclusive until the detection condition and application state are independently validated.
