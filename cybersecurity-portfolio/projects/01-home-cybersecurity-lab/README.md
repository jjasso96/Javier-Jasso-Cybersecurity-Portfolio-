# Project 1: Virtual Cybersecurity Lab on Apple Silicon

**Project type:** Personal cybersecurity home lab  
**Status:** Core lab setup completed; evidence collection and network configuration verification pending  
**Environment:** Apple M3 Mac, UTM, Kali Linux ARM64, Ubuntu Server

## Overview

I built a personal virtualized environment to develop practical cybersecurity skills, gain experience with Linux administration, and troubleshoot a web application security lab.

The project involved configuring virtual machines on Apple Silicon, working through Linux and web application setup issues, and accessing Damn Vulnerable Web Application (DVWA) in a controlled learning environment.

This project emphasizes hands-on troubleshooting, technical documentation, and establishing a foundation for future vulnerability assessment and security testing.

## Objectives

- Configure and use Linux virtual machines on Apple Silicon.
- Develop familiarity with Linux command-line administration and troubleshooting.
- Work through web server and application dependency configuration.
- Access DVWA and explore its application interface and security settings.
- Establish a documented foundation for future, controlled web application security testing.

## Environment and Technologies

| Component | Purpose |
|---|---|
| Apple M3 Mac | Host computer |
| UTM | Virtual machine management |
| Kali Linux ARM64 | Cybersecurity learning environment |
| Ubuntu Server | Linux server environment |
| Apache, MariaDB, PHP | Web application stack components used during setup |
| DVWA | Intentionally vulnerable web application for security training |

**Network configuration note:** The virtual machines' networking mode and isolation controls have not yet been verified. Network architecture and isolation will be documented after reviewing the actual UTM settings.

## Implementation and Work Completed

### 1. Virtualization and Linux

- Configured virtual machine resources in UTM on Apple Silicon.
- Installed and accessed Linux virtual machine environments.
- Worked through installation and configuration issues during setup.
- Gained practical experience navigating Linux environments and troubleshooting system behavior.

### 2. Web Application Environment

- Worked through Apache, MariaDB, and PHP configuration during the DVWA setup.
- Troubleshot web server and application configuration issues.
- Resolved setup obstacles sufficiently to access the DVWA web interface.

### 3. DVWA Interface

- Successfully accessed DVWA and logged in.
- Navigated the application interface and its security settings.
- Established a starting point for future controlled security testing.

**Testing status:** Specific vulnerability tests, exploitation results, findings, and remediation outcomes have not yet been documented as verified results. No vulnerability findings are claimed in this case study.

## Troubleshooting and Lessons Learned

The setup process required working through virtualization, Linux, web server, and application configuration issues.

Key lessons from the project include:

- Troubleshooting requires identifying the failing component rather than assuming the entire environment is broken.
- Web applications depend on multiple services and configuration layers working together.
- Verifying application accessibility is an important setup milestone, but it does not establish that security testing has been completed.
- Technical documentation should distinguish observed behavior from assumptions and unverified configurations.
- Running virtual machines on Apple Silicon can introduce architecture and compatibility considerations that must be accounted for during setup.

## Security Considerations

- Use DVWA only in an authorized, controlled lab environment.
- Verify VM networking and isolation before conducting further security testing.
- Do not expose the intentionally vulnerable application to the public internet.
- Avoid including passwords, tokens, private IP details, or other sensitive information in published screenshots.
- Record test procedures and results before making security claims.

## Skills Practiced

- Virtualization with UTM
- Linux environment setup and troubleshooting
- Web server and application stack configuration
- Web application navigation and security settings
- Technical documentation and evidence-based reporting
- Security lab planning and risk awareness

## Next Steps

- [ ] Verify and document UTM networking mode for each VM.
- [ ] Confirm network isolation and document the actual lab topology.
- [ ] Capture sanitized screenshots of the VM configuration and working DVWA interface.
- [ ] Record the specific DVWA security level selected during testing.
- [ ] Conduct authorized, controlled tests against selected DVWA modules.
- [ ] Document test procedures, observations, expected behavior, and remediation guidance.
- [ ] Update this report only when results and supporting evidence are available.

## Evidence and References

**Current evidence status:** No supporting screenshots or exported test results have been collected for this report.

Future evidence should include sanitized VM configuration screenshots, proof of DVWA access, relevant test observations, and a network diagram based on verified configuration.

**Project outcome:** A working starting point for hands-on cybersecurity learning, with further validation, security testing, and evidence collection remaining.
