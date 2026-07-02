# SOAR Automated Incident Response Lab

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
