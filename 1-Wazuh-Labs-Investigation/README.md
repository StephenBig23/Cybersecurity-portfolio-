# Wazuh Labs & Investigations

This section documents authorized Wazuh lab exercises and alert investigations. It focuses on converting telemetry into defensible findings, improving detection coverage, and recording repeatable analysis workflows.

## Suggested structure

```text
1-Wazuh-Labs-Investigation/
├── README.md
├── labs/
│   └── <lab-name>/
│       ├── README.md
│       ├── screenshots/
│       └── evidence/
├── investigations/
│   └── <case-name>/
│       ├── README.md
│       ├── timeline.md
│       └── iocs.md
└── detection-content/
    ├── rules/
    ├── decoders/
    └── queries/
```

Create only the folders and artifacts that are relevant to a documented exercise. Do not commit raw sensitive logs, production configuration, credentials, or unredacted screenshots.

## Lab write-up template

Copy this outline into each lab or investigation `README.md`:

```md
# <Lab or investigation title>

## Objective
What question, alert, or detection scenario was investigated?

## Scope and authorization
Describe the isolated lab or authorized environment. Do not include sensitive asset details.

## Environment
- Wazuh version:
- Data sources / agents:
- Supporting tools:
- Relevant ATT&CK techniques (if applicable):

## Procedure
1. 
2. 
3. 

## Detection or investigation logic
Include sanitized Wazuh rules, queries, decoder examples, or triage steps.

## Evidence and findings
Summarize meaningful events, correlations, and validation steps. Link only to redacted supporting artifacts.

## Outcome and improvements
Document the result, tuning performed, false-positive considerations, and follow-up work.
```

## Investigation checklist

- [ ] Confirm the alert source, time range, severity, affected asset label, and initial event context.
- [ ] Preserve a sanitized record of relevant events and correlate related telemetry.
- [ ] Determine whether the activity is expected, benign but noisy, suspicious, or confirmed malicious.
- [ ] Map validated behavior to MITRE ATT&CK only when the mapping is supported by evidence.
- [ ] Record containment or remediation recommendations appropriate to the lab scenario.
- [ ] Note rule-tuning opportunities and validation results.

## Useful artifacts

| Artifact | Purpose |
| --- | --- |
| Alert triage notes | Captures initial context, analyst decisions, and escalation rationale |
| Timeline | Shows how related events unfolded over time |
| Detection rule | Documents logic used to identify a behavior |
| Decoder or parser note | Explains how a custom log format is normalized |
| Dashboard screenshot | Demonstrates visibility after redaction |
| Tuning record | Tracks false-positive reduction and regression testing |

## Publication guidance

Use synthetic data or sanitize artifacts before committing them. Describe commands and configurations at a level that demonstrates the work while avoiding disclosure of real infrastructure or secrets.
