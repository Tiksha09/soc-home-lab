# Lab Setup

## Ubuntu

- Installed Wazuh Manager
- Installed Wazuh Dashboard
- Verified services

```bash
sudo /var/ossec/bin/wazuh-control status
```

---

## Kali

Connected to the same VMware NAT network.

Verified connectivity:

```bash
ping 192.168.162.133
```

---

## Generated Security Events

- SSH authentication failures
- Network reconnaissance using Nmap

---

## Investigated

Used Wazuh Threat Hunting to analyze:

- Rule IDs
- Severity
- MITRE ATT&CK mapping
