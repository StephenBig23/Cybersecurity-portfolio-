# Incident Response & Threat Hunting

This section contains authorized incident-response exercises and proactive threat hunts. The goal is to demonstrate a disciplined process: build a hypothesis, collect and validate evidence, document decisions, and improve defenses.

## Suggested structure

```text
2-Incident-Response-Threat-Hunting/
├── README.md
├── incident-response/
│   └── <case-name>/
│       ├── README.md
│       ├── timeline.md
│       ├── indicators.md
│       └── lessons-learned.md
├── threat-hunts/
│   └── <hunt-name>/
│       ├── README.md
│       ├── hypothesis.md
│       └── queries/
└── playbooks/
    └── <playbook-name>.md
```

## Incident-response case template

```md
# <Case title>

## Executive summary
Provide a concise, sanitized summary of the scenario, impact, and result.

## Scope and authorization
State that the activity occurred in an authorized lab or approved environment.

## Timeline
| Time (UTC) | Event | Source | Analyst action |
| --- | --- | --- | --- |
| | | | |

## Analysis
- Initial alert or report:
- Affected system labels:
- Evidence reviewed:
- Key findings:
- Confidence and limitations:

## Response actions
Describe containment, eradication, recovery, and validation actions relevant to the scenario.

## Recommendations
List prioritized improvements to logging, detection, hardening, processes, or user awareness.

## Lessons learned
Capture what worked, what was missing, and what should be tested next.
```

## Threat-hunt template

```md
# <Hunt title>

## Hunt hypothesis
State a testable behavior-based hypothesis, not just an indicator search.

## Data sources and scope
List the authorized telemetry, time period, asset groups, and known coverage gaps.

## Method
Explain the pivot strategy, analytics, queries, and validation steps.

## Findings
Summarize positive, negative, and inconclusive results with supporting sanitized evidence.

## Detection opportunities
Identify analytics, rules, baselines, or telemetry changes that would improve visibility.

## Follow-up
Record investigations, tuning, or collection improvements that should occur next.
```

## Response lifecycle reference

1. **Preparation** — Validate tools, logging, roles, communication paths, and evidence handling.
2. **Identification** — Triage reports and alerts; establish scope and confidence.
3. **Containment** — Limit impact while preserving the evidence needed for analysis.
4. **Eradication** — Remove the cause and close persistence paths.
5. **Recovery** — Restore systems safely and monitor for recurrence.
6. **Lessons learned** — Improve detections, runbooks, architecture, and training.

## Quality checklist

- [ ] Scope and authorization are stated.
- [ ] Times use a clear time zone, preferably UTC.
- [ ] Claims are distinguished from evidence and analyst hypotheses.
- [ ] Indicators are sanitized and include context, not just a list of values.
- [ ] Queries are documented with their data source and interpretation.
- [ ] Recommendations are specific, prioritized, and defensible.
