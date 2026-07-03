# Security Operations: What a SOC Actually Does

## Overview

Security Operations (SecOps) is the function that watches systems, catches suspicious activity, and responds before it becomes damage. This document breaks down how a Security Operations Center (SOC) runs, day to day, and why the workflow matters to anyone assessing risk or reviewing a breach after the fact.

## What a SOC Is For

A SOC exists to answer three questions on every alert:

1. Is something suspicious happening?
2. Is it a real problem?
3. What should be done about it?

A SOC does not stop every attack. It makes sure attacks get caught and handled instead of sitting unnoticed. That distinction matters for anyone assessing an organization's security posture: the question is never "did something happen," it's "how fast was it caught and what happened next."

## What Gets Monitored

- User logins and access activity
- Network traffic
- Applications
- Cloud systems
- Servers and endpoints

## Who Handles What

| Role | What they actually do |
|---|---|
| Tier 1 Analyst | First eyes on the alert. Checks context, follows the playbook, escalates what needs escalating, writes the summary |
| Tier 2 / Senior Analyst | Digs into the complex cases, runs deeper investigation, leads response |
| SOC Manager / Lead | Runs the operation, coordinates response, reports up to leadership |

A Tier 1 analyst is not expected to solve everything. They are expected to recognize what matters, document it clearly, and escalate correctly. That's a lower bar than people assume, and a higher one than most give it credit for: clean documentation under time pressure is a real skill, not a formality.

## Why This Matters Beyond the SOC

Every incident summary a SOC produces becomes evidence somewhere else: in a breach notification decision, an audit response, or a board update. A privacy or compliance function that can't read a SOC alert accurately will either overreact to noise or miss a real problem hiding in the details. Reading these reports is not a technical skill on its own; it's a risk-interpretation skill, and it's the same one used to read a regulatory finding or an audit exception.

## Frameworks Referenced

- NIST Cybersecurity Framework (Detect, Respond functions)
- PHIPA and PIPEDA breach assessment context
- OPC guidance on incident documentation
