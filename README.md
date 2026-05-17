# Cowrie SSH Honeypot Lab

## Overview
A beginner honeypot lab using Cowrie to simulate an SSH server, 
monitor unauthorized access attempts, and analyze attacker behavior patterns.

## Environment
- **Host Machine:** MacBook Air (Intel Core i5, 8GB RAM)
- **Honeypot Tool:** Cowrie 2.9.19
- **Language:** Python 3.11
- **Platform:** macOS (local deployment)

## What Was Built
- Installed and configured Cowrie SSH honeypot
- Deployed fake SSH server listening on port 2222
- Simulated attacker login attempts and captured credentials
- Monitored real-time logs of attacker behavior
- Analyzed commands run by attacker inside fake shell environment

## What the Logs Captured
- Source IP addresses of connection attempts
- SSH client fingerprints (hassh)
- Credential attempts (username/password combinations)
- Authentication failures and successes into fake shell
- Every command run by attacker inside honeypot including:
  - whoami
  - ls
  - cat /etc/passwd (attempt to read password file)

## Key Concepts Demonstrated
- Honeypot deployment and monitoring
- Attacker behavior analysis
- SSH protocol and authentication patterns
- Log analysis and threat intelligence
- Deception-based security techniques

## Key Findings
- Attackers immediately attempt to read /etc/passwd after gaining access
- Common credentials used: root​​​​​​​​​​​​​​​​
