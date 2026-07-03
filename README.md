# SOAR Automated Incident Response Lab

![SOAR](https://img.shields.io/badge/SOAR-Automation-blue)
![Wazuh](https://img.shields.io/badge/Wazuh-SIEM-green)
![Shuffle](https://img.shields.io/badge/Shuffle-Orchestration-orange)
![TheHive](https://img.shields.io/badge/TheHive-Case_Management-yellow)
![FortiGate](https://img.shields.io/badge/FortiGate-Firewall-red)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE-ATT%26CK-purple)
![License](https://img.shields.io/badge/License-MIT-lightgrey)
## Wazuh • Shuffle • TheHive • FortiGate

> Automated Incident Response Playbooks for Brute Force, Phishing, and Malicious PowerShell Incidents.

---

## Overview

This project demonstrates how to build an automated Security Orchestration, Automation, and Response (SOAR) workflow in a home SOC environment.

The objective is to automate the incident response lifecycle—from alert generation and investigation to IOC enrichment, case management, containment, and analyst notification.

Instead of performing incident response manually, this lab orchestrates multiple security tools to reduce response time and improve operational efficiency.

---

## Objectives

- Build a production-like SOAR lab
- Automate incident response workflows
- Integrate Wazuh with Shuffle
- Create cases automatically in TheHive
- Enrich IOCs using external threat intelligence
- Perform automated containment actions
- Generate analyst notifications
- Document every automation workflow

---

## Lab Components

| Component | Purpose |
|------------|----------|
| Wazuh | SIEM / Detection |
| Sysmon | Windows telemetry |
| Windows 10 | Endpoint |
| Kali Linux | Attack machine |
| Shuffle | SOAR Platform |
| TheHive | Incident Management |
| VirusTotal API | IOC enrichment |
| AbuseIPDB API | IP reputation |
| URLHaus API | Malicious URL lookup |
| FortiGate | Automated containment |

---

## Incident Response Workflow

```text
Attack

↓

Detection (Wazuh)

↓

Automation Trigger (Shuffle)

↓

IOC Enrichment

↓

Decision

↓

Create Case (TheHive)

↓

Containment

↓

Notification

↓

Incident Closure
```

---

## Automated Playbooks

### Brute Force Response

```
SSH Brute Force

↓

Detect Login Failures

↓

Extract Source IP

↓

AbuseIPDB Lookup

↓

Create TheHive Case

↓

Block IP (FortiGate)

↓

Notify Analyst
```

---

### Phishing Response

```
Suspicious Email

↓

Extract URL

↓

VirusTotal

↓

URLHaus

↓

Create Case

↓

Tag IOC

↓

Notify Analyst
```

---

### Malicious PowerShell Response

```
PowerShell Detection

↓

Extract Hash

↓

VirusTotal

↓

Create Case

↓

Containment

↓

Notify Analyst
```

---
