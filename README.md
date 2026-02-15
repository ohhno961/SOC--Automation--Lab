# 🤖 SOC Automation Lab: Automated Incident Response (SOAR + EDR)
## Overview
This repository documents the implementation of enterprise-grade automated incident response pipelines. The goal of these projects was to move beyond manual alert triage by building "self-healing" workflows that connect EDR (Endpoint Detection & Response) telemetry with SOAR orchestration to isolate threats in real-time.

##  🚀 Project 1: LimaCharlie + Tines Integration (Cloud-Native SOAR)
Objective: Built a fully automated detection-to-response pipeline to reduce "Mean Time to Respond" (MTTR) for credential-based attacks.

##  🛠️ Technical Stack
** EDR: ** LimaCharlie

 ** SOAR: **Tines

** Communication:**  Slack, Email (SMTP)

** Threat Simulation:**  LaZagne (Credential Harvesting), PowerShell (Post-Exploitation)

** Infrastructure: ** Windows Server VM (VirtualBox)

##  Key Accomplishments
** Automated Host Isolation:**  Designed a Tines storyboard that triggers an automatic isolation of a Windows endpoint upon detection of credential dumping (LaZagne).

** Enriched Alerting: ** Configured webhooks to send JSON payloads to Slack, providing analysts with instant metadata: file paths, hashes, and command-line arguments.

** Interactive Workflows: ** Implemented "Analyst-in-the-loop" logic, allowing a human to approve or deny an isolation request directly from a Slack notification.

** Detection Engineering:**  Authored custom JSON-based rules in LimaCharlie targeting PowerShell misuse and privilege escalation scenarios.

##  🎣 Project 2: Automating Phishing Response (Cortex XSOAR)
** Objective: ** Investigated and remediated a spear-phishing campaign targeting executive-level users using the industry-leading Palo Alto Networks XSOAR platform.

##  🛠️ Technical Stack
** Platform:**  Cortex XSOAR (Threat Intel Management instance)

** Frameworks:**  NIST Incident Response Lifecycle

** Focus: ** Phishing Analysis & Threat Intelligence

##  Key Accomplishments
** Playbook Execution:**  Leveraged automated playbooks to parse malicious emails, extract indicators (IOCs), and perform reputation lookups.

** War Room Management:**  Utilized the XSOAR War Room for real-time artifact evidence collection and collaborative investigation.

** Incident Reporting:**  Generated comprehensive investigative reports and post-incident summaries for executive stakeholders.

##  🧠 Skills Demonstrated
** API Integration: ** Proficient in connecting security tools via RESTful APIs and Webhooks.

** Logic & Scripting: ** Skilled in JSON/YAML for rule configuration and workflow logic.

** Architectural Mapping: ** Used Draw.io to document complex IR playbooks for auditability and team training.

** Threat Emulation: ** Understanding of adversary behavior to validate detection accuracy.
