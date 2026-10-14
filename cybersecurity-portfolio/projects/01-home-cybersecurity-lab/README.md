# Project 1: Virtual Cybersecurity Lab on Apple Silicon

**Project type:** Home lab / Linux administration / Web application security  
**Status:** Lab configured; additional evidence and validation pending  
**Environment:** Apple M3 Mac, UTM, Kali Linux ARM64, Ubuntu Server

## Overview

I built a personal virtualized environment to develop practical cybersecurity skills, troubleshoot Linux systems, and explore web application security in a controlled lab.

The project involved configuring virtual machines on Apple Silicon, working with web application dependencies, and deploying Damn Vulnerable Web Application (DVWA) for security learning.

A key part of this project was troubleshooting configuration and application-access issues until I could access the DVWA interface and use its security-level settings.

## Objectives

- Build a practical cybersecurity learning environment on Apple Silicon.
- Gain hands-on experience with Linux virtual machines and system services.
- Configure the components required to run DVWA.
- Develop troubleshooting skills through installation and application-access issues.
- Establish a foundation for future web vulnerability testing and security analysis.

## Environment and Technologies

| Component | Purpose |
|---|---|
| Apple M3 Mac | Host computer |
| UTM | Virtual machine management |
| Kali Linux ARM64 | Cybersecurity learning environment |
| Ubuntu Server | Linux server administration |
| Apache | Web server |
| MariaDB | Database service |
| PHP | Server-side application runtime |
| DVWA | Deliberately vulnerable web application for authorized security practice |

**Networking note:** The original VM networking mode and isolation configuration have not yet been verified. They will be documented after reviewing the UTM settings.

## Implementation and Work Completed

### 1. Virtualization and Linux

- Configured virtual machines in UTM on an Apple Silicon Mac.
- Installed and accessed Kali Linux ARM64 and Ubuntu Server.
- Worked through installation and configuration issues during setup.
- Gained practical experience navigating Linux environments and troubleshooting system behavior.

### 2. Web Application Stack

- Worked with Apache, MariaDB, and PHP while configuring DVWA.
- Investigated web server, PHP, and application configuration issues.
- Troubleshot application directory and service-access problems.
- Verified that the DVWA web interface was accessible.

### 3. DVWA Interface

- Accessed the DVWA interface after troubleshooting the setup.
- Used the application's security-level settings.
- Established a starting point for controlled web application security exercises.

Individual vulnerability tests, findings, and remediation outcomes are not included here because they have not yet been documented and verified.

## Troubleshooting and Lessons Learned

This project required more than installing software. I had to investigate configuration issues across the virtual machine, Linux services, application dependencies, and web application itself.

The experience reinforced several practical troubleshooting principles:

- Verify service status and configuration instead of assuming a service is working.
- Separate operating system, web server, PHP, database, and application-level problems.
- Validate changes by checking the resulting application behavior.
- Record commands, configuration changes, and successful outcomes so issues can be reproduced.
- Verify network exposure and isolation before conducting security testing.

**Documentation improvement:** Exact commands, error messages, and resolution steps will be added after reviewing available terminal history or reproducing the relevant steps.

## Security Considerations

- Use DVWA only in an environment you own or are explicitly authorized to test.
- Verify VM networking and isolation before conducting vulnerability testing.
- Do not expose DVWA to the public internet.
- Use non-sensitive lab credentials and avoid publishing passwords, tokens, or private network details.
- Keep screenshots and configuration examples sanitized before publishing them.
- Document the scope of each security test and distinguish observations from confirmed findings.

## Cybersecurity Skills Demonstrated

- Linux installation and basic system administration
- Virtualization and environment configuration
- Web server and application dependency troubleshooting
- Basic web application deployment
- Evidence-based technical documentation
- Security lab setup and safe testing awareness

## Next Steps

- [ ] Verify UTM network mode and document the actual configuration.
- [ ] Capture sanitized screenshots of the virtual machines and working DVWA interface.
- [ ] Record relevant troubleshooting commands and verified resolutions.
- [ ] Document individual DVWA security exercises, including test objective, observed behavior, and security implications.
- [ ] Add remediation guidance and retest results where applicable.
- [ ] Create an architecture diagram based on the verified configuration.

## Project Outcome

I successfully configured a personal virtual cybersecurity lab and accessed DVWA, including its security-level settings. The project provided practical experience with Linux environments, web application dependencies, and troubleshooting.

The next phase is to strengthen the documentation with reproducible evidence and verified security testing results.

