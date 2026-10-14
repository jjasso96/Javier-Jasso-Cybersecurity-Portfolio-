# Project 1: Virtual Cybersecurity Lab on Apple Silicon

**Project type:** Personal cybersecurity home lab  
**Environment:** Apple M3 Mac, UTM, Kali Linux ARM64, Ubuntu Server  
**Status:** Linux VM setup and troubleshooting completed; network configuration and supporting evidence still need verification

## Overview

I set up a personal virtualized environment to practice Linux administration and work through a web application security lab. The project involved configuring virtual machines on Apple Silicon, troubleshooting Linux and web-stack setup issues, and reaching the DVWA application interface.

This case study focuses on the environment setup and troubleshooting process. It does not claim a verified network topology or completed security test results.

## Objectives

- Configure and access Linux virtual machines on Apple Silicon.
- Practice Linux environment setup and troubleshooting.
- Work through web server and application dependency issues.
- Access DVWA and explore its interface and security settings.
- Establish a starting point for future authorized security testing.

## Environment and Technologies

| Component | Role in the lab |
|---|---|
| Apple M3 Mac | Host computer |
| UTM | Virtual machine management |
| Kali Linux ARM64 | Cybersecurity learning environment |
| Ubuntu Server | Linux server environment |
| Apache, MariaDB, PHP | Web application stack components used during setup |
| DVWA | Intentionally vulnerable application used for security learning |

**Network configuration:** The VM networking mode, connectivity between machines, and isolation controls have not been verified from retained settings. No network topology is asserted in this report.

## Work Completed

### Virtualization and Linux

- Configured virtual machine resources in UTM on Apple Silicon.
- Installed and accessed Linux virtual machine environments.
- Worked through installation and configuration issues during setup.
- Practiced navigating Linux environments and troubleshooting system behavior.

### Web Application Setup

- Worked through Apache, MariaDB, and PHP configuration during DVWA setup.
- Troubleshot web server and application configuration issues.
- Resolved setup obstacles sufficiently to access the DVWA interface.

### DVWA Access

- Accessed and logged into DVWA.
- Navigated the application interface and its security settings.

**Testing status:** The activities above establish setup and interface access. They do not establish that a specific vulnerability test, exploitation attempt, or remediation was completed. No such results are claimed here.

## Troubleshooting Lessons

- Identify which component is failing rather than assuming the entire environment is unavailable.
- Web applications depend on multiple services and configuration layers.
- Application accessibility is a setup milestone, not proof that security testing has been performed.
- Record observed behavior separately from assumptions about configuration.
- Apple Silicon virtualization may introduce architecture and compatibility considerations.

## Security Considerations

- Use DVWA only in an authorized, controlled lab.
- Verify networking and isolation before conducting further tests.
- Do not expose the intentionally vulnerable application to the public internet.
- Sanitize screenshots to remove credentials, tokens, and sensitive system details.
- Record procedures and evidence before making security claims.

## Skills Practiced

- UTM virtualization and VM setup
- Linux installation and troubleshooting
- Web server and application-stack troubleshooting
- DVWA interface navigation and security-settings familiarization
- Technical documentation and evidence-conscious reporting
- Security lab planning and risk awareness

## Next Steps

- [ ] Inspect and record the actual UTM networking mode for each VM.
- [ ] Verify connectivity and isolation before further security testing.
- [ ] Capture sanitized screenshots of VM settings and the working DVWA interface.
- [ ] Record the DVWA security level actually selected.
- [ ] Perform an authorized test against a selected DVWA module.
- [ ] Document the procedure, observed result, analysis, and relevant remediation guidance.
- [ ] Update this case study only when the additional work is verified.

## Evidence and References

**Current evidence status:** No supporting screenshots or exported test results are currently retained for this report.

Potential future evidence includes sanitized VM configuration screenshots, proof of DVWA access, test observations, and a network diagram based on verified settings. These are planned evidence items, not files currently available.

**Current outcome:** A usable starting point for hands-on cybersecurity learning, with network verification, structured security testing, and evidence collection still outstanding.
