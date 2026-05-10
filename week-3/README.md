# Threat Identification & Social Engineering in Practice
### SCWIST Cybersecurity Program — Week 3 | Daphne Obadan

---

I spent 7+ years in compliance and risk across healthcare, government, and telecoms
before entering cybersecurity. That background changes how I read every threat scenario.
This is Week 3 of my SCWIST training. What follows is not a course summary.
It is how I am translating formal learning into applied, role-ready thinking.

---

## Why This Week Matters to a Security Team

Most breaches do not start with a zero-day exploit. They start with a person making
a reasonable decision under pressure, with incomplete information, in a manipulated context.

Week 3 focused on that exact problem: understanding what threats actually are,
how attackers engineer human behaviour to exploit them, and what the response
infrastructure looks like across security roles.

The instructor's line that reframed everything: *"A threat isn't always technical."*

---

## Applied Role Mapping

This is where I focused my energy. Understanding a concept matters less than knowing
which function owns it, which team responds, and where I fit.

| Threat Scenario | Role Responsible | What That Role Actually Does |
|---|---|---|
| Staff member reports a suspicious email | SOC Analyst (Tier 1) | Triages the alert, pulls headers and metadata, assesses severity, escalates if confirmed |
| User clicked a link before reporting it | Help Desk + SOC | Isolates the session, resets credentials, opens an incident ticket, documents the timeline |
| Same phishing theme appearing across 3 departments | Security Awareness Coordinator | Identifies the pattern, updates training content, runs a targeted simulation for affected teams |
| Incident needs to be logged for audit | GRC / Compliance Assistant | Documents the event chain, maps it to policy, prepares evidence for the audit trail |

I have done the GRC column before. Governance, documentation, and audit readiness are not
abstract to me. My NHS and LASEPA work was largely about maintaining exactly this kind of
evidence trail under regulatory scrutiny.

---

## Threat Anatomy: What I Actually Needed to Understand

A threat has two components. Get one wrong and your risk assessment falls apart.

**Asset** — what has value and needs protecting (data, access, systems, reputation)
**Vulnerability** — the weakness that leaves the asset exposed

Risk lives where those two things meet. My homework this week asked me to define
what a vulnerability is and frame risk as a question. My answer:

> A vulnerability is a weakness. Risk is asking: how likely is this threat to exploit
> this weakness, and what is the impact if it does?

That framing is directly applicable to GRC work — it is essentially how a risk register
gets populated.

---

## Phishing Variants: Recognising the Pattern Across Channels

| Variant | Channel | What Makes It Effective |
|---|---|---|
| Phishing | Email | Volume. Most land somewhere. Some always get clicked. |
| Spear Phishing | Email (targeted) | The attacker knows enough to sound credible. CEO fraud runs on this. |
| Smishing | SMS / text | People respond to texts faster and with less scrutiny than email |
| Vishing | Voice call | Real-time pressure makes verification feel awkward or slow |

The common thread across all four: they manufacture urgency, exploit trust, and
target the moment between receiving a message and thinking about it.

The simple detection rule I wrote in my notes: **unexpected + urgent + sensitive = pause and verify.**

---

## Social Engineering: The Emotional Layer

Attackers are not guessing. They are selecting from a known list of reliable triggers.

`Urgency` `Fear` `Scarcity` `Authority` `Helpfulness` `Curiosity` `Social Pressure`

Training yourself to notice the emotion first, before engaging with the content, is
the actual skill. In a compliance context, I would frame this as: the emotional state
the message creates is the control you need to override.

In a SOC or awareness role, knowing these triggers is how you build detection logic
and design effective simulations.

---

## What to Do When You Spot an Attack

The response sequence matters as much as the detection:

1. Report quietly. Do not alert the sender.
2. Capture everything before touching it: screenshot, sender address, timestamp, message content.
3. Preserve the original. Do not delete before the SOC or security team has reviewed it.
4. If you already clicked: report immediately. Do not wait. Time is a containment variable.
5. Follow the organisation's incident response procedure. This is not optional.

The instinct to handle it yourself is exactly what makes incidents worse.

---

## What I Am Building Toward

I am targeting GRC Analyst, Compliance Analyst, Privacy Assistant and Security Awareness Coordinator
in the Canadian tech sector.

---

*SCWIST Cybersecurity Scholar 2026 | Toronto, ON*
*[linkedin.com/in/daphne-obadan](https://linkedin.com/in/daphne-obadan)*
*GitHub portfolio updated weekly throughout April–August 2026*
