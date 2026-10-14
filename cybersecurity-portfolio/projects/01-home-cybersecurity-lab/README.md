# Project 1: Virtual Cybersecurity Lab on Apple Silicon

**Project type:** Personal cybersecurity home lab  
**Environment:** Apple M3 Mac, UTM, Kali Linux ARM64, Ubuntu Linux  
**Status:** VM setup, SSH connectivity checks, and an initial firewall rule change documented; firewall enforcement and network isolation remain unverified

## Overview

I built a small virtualized lab to practice Linux administration, network discovery, remote administration, and web application security. The screenshots show Kali Linux communicating with an Ubuntu virtual machine, an SSH connection, an Nmap service scan, and an attempted UFW rule change.

This is a learning lab, not a production environment. The published report deliberately omits exact IP addresses, account names, MAC addresses, SSH key fingerprints, and other host-identifying details. Raw screenshots are not embedded because they contain sensitive lab details.

## Objectives

- Configure and access Linux virtual machines on Apple Silicon.
- Practice basic network troubleshooting and service discovery.
- Establish SSH connectivity between lab systems.
- Explore host firewall rule management with UFW.
- Keep test observations separate from conclusions that still need verification.

## Environment and Tools

| Component | Role |
|---|---|
| Apple M3 Mac and UTM | Host and virtualization platform |
| Kali Linux | Security testing and network diagnostics |
| Ubuntu Linux | Lab system used for SSH and firewall practice |
| `ping` | Basic IP reachability check |
| Nmap | Service discovery |
| OpenSSH client/server | Remote shell connectivity |
| UFW | Host firewall rule management |
| DVWA | Intentionally vulnerable web application used in a separate lab exercise |

The screenshots show two Linux virtual machines with private lab networking. The exact addresses and host identifiers are intentionally excluded from this public report. The full network topology and UTM isolation settings have not been verified.

## Work Completed and Observations

### 1. Network reachability

- Used `ip a` on Ubuntu to inspect its network interfaces and assigned addresses.
- From Kali, sent ICMP echo requests to the Ubuntu lab system.
- The displayed ping statistics reported replies and no packet loss during that captured test.

**What this establishes:** The two lab systems had IP-level reachability at the time of the test. It does not independently establish the full network topology, segmentation, or isolation from other networks.

### 2. Service discovery

- Ran an Nmap service/version scan against the authorized Ubuntu lab system.
- The captured output reported TCP port 22 open and identified an OpenSSH service associated with Ubuntu.
- The scan also reported other probed ports as filtered/no-response.

The target address and detailed host identifiers are intentionally omitted. The screenshot is a point-in-time observation, not a complete security assessment or proof that the host is hardened.

### 3. SSH connectivity

- Connected from Kali to the Ubuntu lab system using SSH.
- Encountered the first-connection host-key prompt and accepted the presented key during the exercise.
- The screenshot then shows a successful login and Ubuntu login banner.

In a real environment, verify an SSH host-key fingerprint through a trusted channel before accepting it. The fingerprint and account details from these screenshots are not reproduced here.

### 4. UFW firewall rule

- Entered a UFW command to deny inbound SSH traffic on TCP port 22.
- After several sudo authentication failures, the terminal displayed “Rule updated” messages for the rule.

**Validation limitation:** The screenshots do not prove that the rule blocked a new SSH connection. Other captured material shows an SSH session succeeding, and the sequence does not establish a controlled before/after connectivity test. Therefore, this project records the rule change as attempted/applied by UFW, but does not claim that SSH access was successfully blocked or that the firewall configuration was fully validated.

Before repeating this exercise, ensure console access is available so a firewall change cannot accidentally lock you out of the VM. If SSH is needed for administration, plan and test the rule carefully.

## Troubleshooting Lessons

- A successful ping confirms reachability, not that a particular TCP service is available.
- Nmap output is a point-in-time view and should be interpreted within the scan scope.
- SSH host-key prompts are a security check; verify fingerprints rather than blindly accepting keys.
- A firewall command reporting success is not the same as validating the intended traffic policy.
- Repeated sudo authentication failures indicate that credentials or authentication state should be checked before continuing.
- Keep raw evidence private when it exposes host identifiers, account names, or other details unnecessary to explain the learning outcome.

## Security Considerations

- Scan only systems explicitly authorized for testing.
- Keep intentionally vulnerable services within a controlled lab.
- Verify UTM network mode and isolation before further testing.
- Do not publish credentials, private keys, session tokens, host fingerprints, or unnecessary network identifiers.
- Avoid firewall changes that could interrupt remote administration; maintain console recovery access.
- Do not claim a control is effective until a deliberate validation test supports that conclusion.

## Skills Practiced

- UTM virtualization and Linux VM setup
- Linux interface inspection with `ip a`
- ICMP reachability checks with `ping`
- Nmap service discovery and basic service identification
- SSH remote access and host-key awareness
- UFW firewall rule management
- Evidence-based technical documentation

## Next Steps

- [ ] Verify UTM network mode, intended topology, and isolation controls.
- [ ] Review the UFW status and numbered rules from the Ubuntu console.
- [ ] Test the firewall policy with a controlled before/after connection check.
- [ ] Confirm SSH host keys through a trusted channel in future sessions.
- [ ] Capture new screenshots with sensitive details removed before capture.
- [ ] Continue authorized DVWA testing and document each test separately.
- [ ] Record exact commands and results only when they can be safely shared and reproduced.

## Evidence and References

**Evidence reviewed:** User-provided screenshots showing Linux interface details, successful ping output, an Nmap result with SSH open, an SSH login, and UFW rule-update output.

**Publication status:** Raw screenshots are not included in the public repository because they contain host and account details. The observations above are sanitized summaries of the visible evidence.

**Current outcome:** Basic lab reachability and SSH connectivity were demonstrated. A UFW rule update was shown, but effective firewall enforcement and overall network isolation remain unverified.
