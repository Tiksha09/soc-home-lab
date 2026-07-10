Wazuh SOC Home Lab
Designed and implemented a Wazuh SIEM home lab using VMware Fusion with Ubuntu Server (Wazuh Manager) and Kali Linux (attacker). Simulated reconnaissance and authentication attacks, analyzed security events using Wazuh Threat Hunting, investigated alerts mapped to the MITRE ATT&CK framework, and developed practical skills in log analysis, threat detection, and incident response.
## Overview

This project demonstrates a Security Operations Center (SOC) home lab built using Wazuh SIEM, Ubuntu Server, and Kali Linux inside VMware Fusion.

The goal was to simulate common attacker activities and investigate the generated security events using the Wazuh Dashboard.

---

## Lab Environment

- Host: macOS (Apple Silicon)
- Hypervisor: VMware Fusion
- SIEM: Wazuh 4.14
- Target: Ubuntu Server
- Attacker: Kali Linux

## Network

Mac (Host)
      |
 VMware NAT
      |
 -----------------------
 |                     |
Ubuntu (Wazuh)      Kali Linux
192.168.162.133

## Attack Scenarios

### 1. SSH Password Guessing

Performed multiple failed SSH login attempts from Kali Linux.

Detection:

- Authentication Failure
- Password Guessing
- SSH

MITRE ATT&CK:

- T1110 - Brute Force

---

### 2. Network Reconnaissance

Executed:

```bash
nmap -sV -A 192.168.162.133
```

Purpose:

- Enumerate open services
- Simulate attacker reconnaissance


## Investigation

Alerts were investigated using:

- Wazuh Threat Hunting
- Alert Severity
- Rule IDs
- Source IP
- MITRE ATT&CK Mapping

## Skills Demonstrated

- SIEM Monitoring
- Threat Hunting
- Linux Administration
- Log Analysis
- SSH Security Monitoring
- MITRE ATT&CK
- VMware Networking
- Incident Investigation


## Screenshots

### Wazuh Dashboard

dashboard.png

### Authentication Failure Detection

![SSH](images/ssh-authentication-failure.png)

### MITRE ATT&CK Mapping

![MITRE](images/mitre-mapping.png)


## Learning Outcomes

This project helped me understand:

- SIEM architecture
- Event collection
- Alert correlation
- Authentication monitoring
- Security event investigation
- Basic SOC analyst workflow# soc-home-lab
Built a Security Operations Center (SOC) home lab using Wazuh SIEM, Ubuntu Server, and Kali Linux on VMware Fusion. Simulated real-world cyber attacks, including SSH password guessing and network reconnaissance, and investigated security alerts through Wazuh Threat Hunting.
