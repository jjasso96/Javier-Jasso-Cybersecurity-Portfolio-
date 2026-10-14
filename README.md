# Project 1: Virtual Cybersecurity Lab on Apple Silicon

**Status:** Lab work completed; evidence and final documentation in progress  
**Environment:** Apple M3 Mac, UTM virtualization, Kali Linux ARM64, Ubuntu Server  
**Focus:** Linux fundamentals, virtualization, troubleshooting, and lab documentation

## Objective

Build a personal, isolated environment for cybersecurity learning and controlled testing on Apple Silicon hardware.

## Environment & Components

- Apple M3 Mac
- UTM virtualization
- Kali Linux ARM64 virtual machine
- Ubuntu Server virtual machine
- Apache web server
- MariaDB
- PHP
- Damn Vulnerable Web Application (DVWA)

The final architecture diagram should reflect the actual VM networking mode and configuration used. Do not assume that the VMs are on a bridged network or that a separate monitoring sensor is present unless verified.

## Work Completed

Based on the lab work performed:

- Configured virtual machine resources and worked through ARM64 compatibility considerations.
- Installed and accessed Linux virtual machines.
- Used Linux command-line tools to troubleshoot services and system configuration.
- Installed/configured components of a web application stack: Apache, MariaDB, and PHP.
- Worked through web server and PHP configuration errors.
- Troubleshot application directory and service-access issues.
- Reached a functioning DVWA application in the lab.

## Troubleshooting Notes to Expand

Add exact commands and screenshots only after reviewing the original terminal history or reproducing the steps.

| Issue | Investigation / resolution to document | Evidence needed |
|---|---|---|
| Linux VM installation/configuration | Record the actual setting or step that resolved it | VM settings screenshot |
| Apache/PHP configuration error | Record the exact error and verified fix | Sanitized terminal output |
| DVWA application access | Document the final service and URL checks used | Browser screenshot and service status |
| VM networking | Record the actual network mode and IP configuration | Sanitized network details |

## Security Considerations

- Keep vulnerable applications confined to a controlled lab.
- Do not expose DVWA to the public internet.
- Use non-sensitive sample credentials.
- Sanitize screenshots before publication.
- Document the network mode and any isolation controls.

## What I Learned

This project reinforced that a cybersecurity lab is not just about installing tools. It requires understanding the operating system, dependencies, services, configuration, networking, and evidence-based troubleshooting.

## Next Steps

- [ ] Add a verified architecture diagram.
- [ ] Add sanitized screenshots of the working VMs and DVWA.
- [ ] Record exact troubleshooting commands and outcomes.
- [ ] Document the actual VM network configuration.
- [ ] Link to the DVWA project report.

## Evidence & References

Add links to relevant official documentation and lab notes here. Do not include screenshots or claims that have not been verified.
