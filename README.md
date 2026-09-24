# Cybersecurity Portfolio

A structured collection of hands-on cybersecurity investigations, incident-response and threat-hunting exercises, network-operations work, and independent projects.

> **Portfolio note:** This repository is designed to document authorized lab work and sanitized technical evidence. Do not upload credentials, private IP addresses, customer data, unredacted logs, malware samples, or packet captures containing sensitive information.

## Portfolio areas

| Area | Focus | Contents |
| --- | --- | --- |
| [1 — Wazuh Labs & Investigations](./1-Wazuh-Labs-Investigation/) | SIEM monitoring, alert triage, rules, and investigations | Lab write-ups, detection logic, dashboards, and sanitized evidence |
| [2 — Incident Response & Threat Hunting](./2-Incident-Response-Threat-Hunting/) | Incident lifecycle, hypothesis-driven hunts, and reporting | Playbooks, hunt reports, timelines, and indicators |
| [3 — Network Operations](./3-Network-Operations/) | Network visibility, troubleshooting, and operational documentation | Diagrams, runbooks, monitoring notes, and change records |
| [4 — Projects](./4-Projects/) | End-to-end security projects | Project briefs, architecture, implementation notes, and outcomes |

## Repository layout

```text
Cybersecurity-portfolio-
├── 1-Wazuh-Labs-Investigation/
├── 2-Incident-Response-Threat-Hunting/
├── 3-Network-Operations/
├── 4-Projects/
└── README.md
```

## Documentation standard

Each published case study should make it easy to understand the work without exposing sensitive data. Use the following structure where applicable:

1. **Objective** — Define the authorized lab scenario, business question, or operational goal.
2. **Environment** — Describe the relevant systems, tools, telemetry, and scope using sanitized details.
3. **Method** — Explain the investigation, hunt, troubleshooting, or implementation process.
4. **Evidence** — Include redacted screenshots, queries, logs, timelines, or diagrams.
5. **Findings** — State what was observed and how it was validated.
6. **Outcome** — Document containment, remediation, improvements, or next steps.
7. **Lessons learned** — Capture detection gaps, operational improvements, and follow-up work.

## Evidence handling

Before publishing, review every artifact for sensitive information:

- Replace real hostnames, usernames, domains, public IP addresses, and asset identifiers with safe labels.
- Remove API keys, passwords, tokens, certificates, and connection strings.
- Sanitize logs and screenshots for personally identifiable information and internal business data.
- Share malware only through approved, controlled channels; use hashes and behavioral summaries in this repository instead.
- Confirm that all work is from an authorized environment.

## Getting started

Browse the sections above to explore the portfolio. Each section contains a guide for organizing future write-ups and supporting materials.

---

*This repository is maintained as an educational and professional portfolio of authorized cybersecurity work.*
