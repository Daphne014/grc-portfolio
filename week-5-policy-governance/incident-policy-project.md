# Week 5 Homework: Policy Creation Exercise

**Program:** SCWIST Cybersecurity Skills for Success — 2026 Cohort
**Organization:** Day 2 Day Communications (D2D) — fictional small Canadian ISP, Ontario
**Policy selected:** Incident Reporting Policy
**Role simulated:** GRC Analyst

> **Instructor feedback incorporated:** Policy language tightened to remove procedure-level detail. CRTC notification updated to reflect triage-first approach. Referenced supporting documents flagged.

---

## The Policy: D2D-SEC-001 Incident Reporting Policy

### Purpose
This policy ensures that when a security incident or data breach occurs at D2D, the right people are notified, legal obligations are met, and the organization can demonstrate accountability.

### Scope
All employees, contractors, and third-party vendors. Covers data breaches, service outages, unauthorized access, and any event affecting emergency services such as 9-1-1 or 9-8-8.

### Expectations
- Report any suspected incident promptly — do not investigate or resolve it independently
- Cooperate honestly with the GRC/IT team during any investigation
- Keep all incident details confidential
- Complete incident reporting training on hire and annually thereafter

### Reporting Requirements

**Internal:** Report to the GRC/IT team as soon as an incident is identified, with enough detail to assess severity and next steps.

**PIPEDA (Canada's federal privacy law):**
- Notify Canada's Privacy Commissioner if a confirmed breach poses real risk of serious harm such as identity theft or financial loss
- Contact affected individuals directly and promptly
- Retain records of all breaches for a minimum of 24 months

**CRTC (Canada's telecom regulator):**
- Notify the CRTC after triage confirms a real major outage,especially where 9-1-1 or emergency services are affected
- Submit a full post-outage report within 30 days of restoration

**Escalation levels:**
- P1 – Critical (ransomware, confirmed breach, 9-1-1 outage): immediate escalation
- P2 – High (suspected unauthorized access, major outage): escalate urgently
- P3 – Medium (minor anomaly, phishing with no data accessed): report promptly

### Referenced Supporting Documents
To be produced separately:
- Incident Report Form
- Incident Response Procedure
- Breach Notification Template (OPC)
- Post-Outage Report Template (CRTC)

---

## Gap Analysis

| Gap Identified | Why It Matters |
|---|---|
| No PIPEDA breach reporting obligations | Without this, D2D has no legal process for notifying the Privacy Commissioner or affected individuals — automatic non-compliance. |
| No CRTC outage notification requirement | No requirement means no accountability when emergency services are disrupted. |
| No breach recordkeeping requirement | PIPEDA requires 24-month retention of all breach records regardless of severity. |
| No escalation structure | Teams have no standard for how fast to respond or who to notify. |
| No emergency service impact criteria | No coverage of incidents affecting 9-1-1, 9-8-8, TTY/IP Relay, or Wireless Public Alerting. |
| No referenced supporting documents | A policy referencing forms that do not exist cannot be operationalized. |

---

## Compliance Mapping

| Policy Section | Regulation | Why this section exists |
|---|---|---|
| Internal Reporting | PIPEDA | Organizations must know a breach occurred before they can act. Without this, nothing else works. |
| Notify Privacy Commissioner | PIPEDA | Canadian law requires reporting breaches that could seriously harm individuals. Staying silent is a legal violation. |
| Notify Affected Individuals | PIPEDA | People whose data was exposed have a right to know so they can protect themselves. |
| Retain Breach Records | PIPEDA | Every breach must be documented for at least 2 years to support accountability and audits. |
| CRTC Outage Reporting | CRTC | As a regulated telecom, D2D must report outages affecting emergency services to the regulator. |
| Escalation Levels | NIST CSF | Not every incident needs the same response. Severity levels ensure the right action happens at the right speed. |

---

## Skills Demonstrated

`Policy gap analysis` `Compliance mapping` `PIPEDA` `NIST CSF` `CRTC regulatory requirements` `Plain language policy writing` `Incident escalation frameworks` `Audit documentation` `GRC analyst workflow`

---

*SCWIST Cybersecurity Scholar 2026 | [linkedin.com/in/daphne-obadan](https://linkedin.com/in/daphne-obadan)*
