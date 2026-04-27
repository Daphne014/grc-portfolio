# Week 1 CIA Triad Analysis: NASA Phishing Incident

**Daphne Obadan · April 2026**  
SCWIST Skills for Success Cybersecurity Program

---

## Incident Identified

**NASA employees duped in Chinese phishing scheme targeting U.S. defense software**  
Source: The Hacker News, April 24, 2026  
Attack period: January 2017 – December 2021

---

## Incident Summary

A Chinese national, Song Wu, an engineer at the Aviation Industry Corporation of
China (AVIC), conducted a multi-year spear-phishing campaign against U.S.
government agencies, universities, and private companies.

By impersonating trusted colleagues and U.S. researchers, Song and his
co-conspirators tricked victims into emailing proprietary software and source
code used for aerospace design and weapons development. Victims included
employees at NASA, the Air Force, the Navy, the Army, and the FAA. Song has been
indicted on wire fraud and aggravated identity theft charges and remains at large.

---

## Impact on the CIA Triad

### Confidentiality — Breached

Confidentiality ensures sensitive information is only accessible to those
authorized to see it. This was the primary target of the attack.

By impersonating legitimate U.S. researchers, Song gained the trust of NASA
employees and other professionals who then voluntarily shared proprietary
software, source code, and sensitive defense technology, information they never
would have disclosed to an unauthorized party. The breach wasn't a technical
hack; it was a social engineering attack that bypassed human judgment.
Confidentiality of export-controlled data was compromised across multiple
agencies and institutions over four years.

### Integrity — Undermined

Integrity refers to the trustworthiness and accuracy of information and the
systems that handle it, including the authenticity of the people involved in
exchanges.

Song fabricated identities to pose as colleagues and engineers. Every email sent
under a false identity was an act of deception that corrupted the integrity of
professional communications. Victims believed they were participating in
legitimate research exchanges; in reality, those interactions had been
compromised from the start. There's also a broader concern: once proprietary
source code leaves a secured environment and reaches an unauthorized actor,
there's no way to verify how it may have been copied, altered, or used.

### Availability — Indirectly Threatened

Availability ensures systems, data, and resources are accessible to authorized
users when needed. This incident didn't directly disrupt operations, but
availability was threatened in a strategic, long-term sense.

The software obtained could enable a foreign state actor to replicate or counter
U.S. defense capabilities. If adversaries use that knowledge to develop
countermeasures or competing systems, they could degrade the operational
advantage these technologies were designed to provide. Once the breach was
discovered, affected organizations would also have needed to audit communication
practices, restrict software-sharing workflows, and potentially overhaul access
controls; all of which impact the availability of normal operations.

---

## Key Lesson

Sophisticated threats don't always require technical intrusion. The weakest link
here was human trust. Effective cybersecurity must address the human layer
through security awareness training, identity verification protocols, and clear
guidelines for sharing sensitive materials not just firewalls and malware
detection.

---

## Connection to My Career Path

As someone pursuing GRC and Policy & Governance roles, this incident is directly
relevant. A Security Policy Coordinator or GRC Analyst would be involved in
designing the exact policies that could have prevented this: export control
training, software-sharing approval workflows, vendor and collaborator
verification procedures, and incident reporting protocols.

This case reinforces why governance and human-centered security awareness are as
critical as any technical control.
