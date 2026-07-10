# Control Mapping, Evidence, and Audit Readiness

## Overview

This document sets out the mechanics of control mapping and evidence management, and how both connect to vendor risk oversight and audit response. These are the working parts behind any claim an organization makes about being "compliant": a risk was identified, a control was put in place, and proof exists that the control functions as intended.

## Controls: What Reduces Risk

A control is anything that reduces risk. It does not eliminate risk; it lowers the likelihood or impact of a given threat to an acceptable level. Controls generally fall into three categories:

- **Technical**: MFA, encryption, logging, access restrictions
- **Administrative**: policies, training programs, approval workflows
- **Operational**: monitoring, periodic reviews, incident response drills

An organization with only technical controls and no administrative or operational layer has gaps that a single tool cannot close. Effective risk management usually requires all three working together.

## Control Mapping

Control mapping is the discipline of connecting three things: a risk, the control that addresses it, and the evidence that proves the control is real and functioning.

Risk → Control → Evidence

This chain is what allows an organization to demonstrate, to a client, regulator, or auditor, that a risk was not only recognized but acted on. Without the evidence step, a control mapping exercise is a set of claims with nothing behind them.

## Evidence

Evidence is proof that a control exists and works. It is what turns a policy statement into something an auditor or client can independently verify.

Common evidence types include:

- MFA configuration exports or screenshots
- Access review logs
- Incident response records
- Signed policy documents with version history
- Training completion records

The operating principle here is straightforward: if it is not documented, it did not happen. Verbal assurance carries no weight in an audit or a client security review. Documentation does.

## Vendor Risk Management

Most organizations depend on a network of external providers: cloud hosting, SaaS platforms, IT managed services, consultants. Each of these vendors touches organizational data in some way, which means each one carries risk the organization cannot fully control directly.

Vendor risk management asks three questions:

- Do our vendors protect our data adequately?
- What happens operationally if a vendor fails or is breached?
- Can the vendor produce evidence of their own controls on request?

This is the reasoning behind security questionnaires, vendor security reviews, and evidence requests during onboarding and renewal cycles. Under PIPEDA, an organization remains accountable for personal information even after it is transferred to a third party for processing, which makes vendor oversight a compliance obligation rather than a courtesy check.

## Cybersecurity Audits

An audit is not an adversarial exercise. It is a structured verification process built around three questions:

- What controls does the organization have in place?
- How does the organization know those controls work?
- Can the organization produce evidence on demand?

Audits exist to build trust between an organization and the parties that rely on it (clients, regulators, insurers), not to catch anyone out. An organization that treats audit prep as an ongoing discipline, rather than a scramble before a review date, is the one that passes without friction.

## Key Takeaways / Recommendations

- Organizations should build control mapping into standard operating procedure, not treat it as a one-time exercise ahead of an audit.
- Evidence collection should be assigned to a specific owner per control; undocumented controls carry the same audit weight as controls that do not exist.
- Vendor risk reviews should be scheduled on a recurring cycle (onboarding, annual renewal, and after any material vendor incident), not left to happen reactively.
- Audit readiness is a continuous operating posture. Organizations that maintain evidence trails year-round face lower disruption and lower risk of findings during formal reviews.

## Frameworks Referenced

- NIST CSF 2.0 (Identify, Protect, Detect, Respond, Recover)
- ISO 27001:2022 Annex A controls
- PIPEDA, Schedule 1, Principle 4.1.3 (accountability for information transferred to third parties)
- OPC guidance on vendor and third-party accountability
