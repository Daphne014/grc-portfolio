# Week 5 Homework: Policy Creation Exercise

**Program:** SCWIST Cybersecurity Skills for Success — 2026 Cohort
**Organization:** Day 2 Day Communications (D2D) — fictional small Canadian ISP, Ontario
**Policy selected:** Incident Reporting Policy
**Role simulated:** GRC Analyst

---

## The Policy: D2D-SEC-001 Incident Reporting Policy

### Purpose
Day 2 Day Communications handles customer data and provides telecommunications infrastructure, including access to emergency services. This policy ensures that when a security incident or data breach occurs, the right people are notified, legal obligations are met, and the organization can demonstrate accountability.

### Scope
This policy applies to all D2D employees, contractors, and third-party vendors who access company systems or customer data. It covers all security incidents including data breaches, service outages, unauthorized access, and any event affecting emergency services such as 9-1-1 or 9-8-8.

### Expectations
All D2D personnel are expected to:

- Report any suspected incident within 1 hour of discovery — do not investigate or attempt to fix it independently
- Use the Incident Report Form or contact the GRC/IT team directly
- Provide honest, accurate information during any investigation
- Keep all incident details confidential unless authorized to share
- Complete incident reporting training on hire and annually thereafter

### Reporting Requirements

**Internal reporting:** All suspected incidents must be reported within 1 hour of discovery, including what happened, when it was noticed, which systems or data may be affected, and any steps already taken.

**PIPEDA obligations (Canada's federal privacy law):**
- Notify the Privacy Commissioner (OPC) if the breach could cause serious harm to individuals — such as identity theft, financial loss, or physical danger
- Contact affected individuals directly and promptly
- Retain records of every breach, including minor ones, for a minimum of 24 months

**CRTC obligations (Canada's telecom regulator):**
- Report major service outages to the CRTC within 2 hours of discovery
- Submit a full post-outage report within 30 days of service restoration
- Any incident affecting 9-1-1 or emergency services is automatically Priority 1

**Escalation tiers:**

| Level | Incident Type | Response Target |
|---|---|---|
| P1 – Critical | Ransomware, confirmed data breach, 9-1-1 outage | Escalate within 15 minutes |
| P2 – High | Suspected unauthorized access, major service outage | Escalate within 1 hour |
| P3 – Medium | Minor system anomaly, phishing attempt (no data accessed) | Report within 4 hours |

---

## GRC Analyst Work: Gap Analysis

Before writing the updated policy, I compared the existing document against current legal and regulatory requirements. Here is what was missing.

| Gap Identified | Why It Matters |
|---|---|
| No PIPEDA breach reporting obligations | Canada's privacy law requires notifying the Privacy Commissioner and affected individuals when a breach poses serious risk of harm. Missing this means automatic non-compliance. |
| No CRTC outage notification timelines | ISPs must report major outages within 2 hours, especially if 9-1-1 services are affected. No timeline means no accountability. |
| No breach recordkeeping requirement | PIPEDA requires organizations to retain records of all breaches for a minimum of 24 months, regardless of severity. |
| No escalation structure | Without defined severity levels, teams have no standard for how fast to respond or who to notify. |
| No emergency service impact criteria | No explicit coverage of incidents affecting 9-1-1, 9-8-8, TTY/IP Relay, or Wireless Public Alerting. |

---

## Compliance Mapping

Linking each policy section to the specific requirement it satisfies — this is what makes a policy audit-ready.

| Policy Section | PIPEDA | NIST CSF |
|---|---|---|
| Internal Reporting | Principle 7 — organizations must have safeguards and awareness of breaches | RS.CO-2: Incidents reported per established criteria |
| Notify Privacy Commissioner | s.10.1 — report breaches posing real risk of significant harm | RS.CO-3: Information shared with appropriate parties |
| Notify Affected Individuals | s.10.1 — direct notification required | RS.CO-4: Coordination with affected stakeholders |
| Retain Breach Records | s.10.3 — minimum 24-month retention | RC.CO-1: Recovery communications managed appropriately |
| CRTC Outage Reporting | Telecom regulatory obligation separate from PIPEDA | RS.CO-2, RC.RP-1: Timely response and recovery execution |
| Escalation Tiers | Principle 7 — risk-appropriate safeguards | RS.AN-1, RS.MI-1: Incidents investigated and contained |

---

## Skills Demonstrated

`Policy gap analysis` `Compliance mapping` `PIPEDA` `NIST CSF` `CRTC regulatory requirements`
`Plain language policy writing` `Incident escalation frameworks` `Audit documentation` `GRC analyst workflow`

---

*SCWIST Cybersecurity Scholar 2026 | [linkedin.com/in/daphne-obadan](https://linkedin.com/in/daphne-obadan)*
