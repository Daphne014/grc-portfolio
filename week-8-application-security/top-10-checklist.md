# Week 8 Homework: Application Security Top 10 Checklist
**Lakeshore Health Technologies | Patient Portal Security Review**
**SCWIST Cybersecurity Scholars Program | June 2026**

---

Lakeshore Health Technologies operates a patient-facing portal that stores and processes personal health information. Under PHIPA and PIPEDA, the organisation has a legal obligation to protect that information with reasonable safeguards. This checklist assesses the portal against the OWASP Top 10, the industry standard for identifying application security risks, and documents the business impact and prevention measure for each.

---

1. Injection

Unvalidated input from users is passed directly into the database. An attacker can manipulate it to extract or delete patient records.

CIA impact: Confidentiality (data exposed), Integrity (records altered or deleted).

Business risk: Mass exposure of personal health information, mandatory breach reporting under PHIPA, and potential regulatory penalties.

Prevention: All user input is validated before processing. Safe database queries are used so user data is never inserted directly.

---

2. Broken Authentication

Weak login controls allow attackers to guess credentials or take over patient accounts. Missing MFA and sessions that never expire are common gaps.

CIA impact: Confidentiality (unauthorised account access), Integrity (data modified by an impersonator).

Business risk: Unauthorised access to health records is a reportable breach. Regulators expect MFA as a baseline for systems holding sensitive data.

Prevention: MFA is enforced on all accounts. Sessions expire after a defined period of inactivity.

---

3. Sensitive Data Exposure

Patient data is stored or transmitted without encryption, leaving it readable if intercepted.

CIA impact: Confidentiality (data exposed in transit or at rest).

Business risk: Unencrypted health data in a breach is difficult to defend to regulators. PHIPA requires appropriate technical safeguards for personal health information.

Prevention: Data is encrypted in storage and in transit. Information no longer needed is deleted on a defined schedule.

---

4. Broken Access Control

Users can access records or functions beyond their permissions. A patient viewing another patient's file is a direct example.

CIA impact: Confidentiality (records visible to unauthorised users), Integrity (data modified without permission).

Business risk: Unauthorised access to personal health information is a PHIPA violation and triggers individual notification obligations.

Prevention: Access is scoped strictly to what each user role requires. Controls are tested before deployment and reviewed on a regular cycle.

---

5. Security Misconfiguration

Systems go live with default credentials, unnecessary features enabled, or incomplete configurations.

CIA impact: Confidentiality and Integrity (open entry points expose data and allow unauthorised changes), Availability (misconfigured systems are more vulnerable to disruption).

Business risk: Avoidable failures carry little regulatory sympathy. Default credentials left unchanged are evidence that basic due diligence was not met.

Prevention: All systems are configured to minimum necessary settings before deployment. Defaults are changed and configurations reviewed after any significant update.

---

6. Vulnerable and Outdated Components

The portal relies on software libraries that are no longer supported or have known, unpatched weaknesses.

CIA impact: All three. An exploited component can expose data, corrupt records, or take systems offline.

Business risk: A breach through a known, unpatched vulnerability is hard to defend. Third-party risk management programs are expected to catch this before it becomes an incident.

Prevention: A component inventory is maintained. Patches are applied promptly. Vendors are assessed to confirm they meet the same standard.

---

7. Identification and Authentication Failures

The portal does not adequately verify who is logging in. Weak password requirements, no account lockout, and inactive session persistence all contribute.

CIA impact: Confidentiality (health records accessed by wrong person), Integrity (records altered under a compromised identity).

Business risk: Attackers can impersonate patients or staff and access health records, widening the scope of any breach and the number of individuals affected.

Prevention: Strong password requirements and MFA are enforced. Inactive sessions are automatically terminated.

---

8. Insecure Design

Privacy and security were not built into the portal from the start. The risk exists in the structure of the system, not just its configuration.

CIA impact: All three, depending on what the design gap exposes. Structural weaknesses rarely affect only one area.

Business risk: Privacy by design is a legal expectation under PHIPA. A system built without it signals a governance failure, and addressing it after deployment is significantly more costly.

Prevention: Privacy impact assessments are completed before development begins. Security requirements are defined at the design stage.

---

9. Insufficient Logging and Monitoring

The portal does not record who accessed what, or those records are not reviewed. Suspicious activity goes undetected.

CIA impact: Availability and Integrity. Without logs, the organisation cannot detect attacks in progress, confirm what data was affected, or respond accurately.

Business risk: Logs are evidence. Without them, the organisation cannot report a breach accurately, identify who was affected, or demonstrate to regulators that it can detect and respond to incidents.

Prevention: Logging is enabled for all access to patient data. Logs are retained for a defined period and reviewed on a regular basis.

---

10. Server-Side Request Forgery (SSRF)

An attacker tricks the portal into making requests to internal systems on their behalf, using it as a gateway to infrastructure it should not reach.

CIA impact: Confidentiality (internal credentials and data exposed), Availability (internal systems disrupted through unintended access).

Business risk: In a cloud-hosted environment, this can expose internal credentials and configuration data, expanding a breach well beyond the portal itself.

Prevention: The application is restricted to a defined list of approved addresses. Input that directs network requests is validated before it is processed.

---

*Part of the SCWIST 2026 Skills for Success Cybersecurity Scholars Program.*
