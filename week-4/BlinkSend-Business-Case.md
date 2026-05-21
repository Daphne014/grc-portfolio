# BlinkSend: Framework Selection & Business Case
**SCWIST Cybersecurity Program | Week 4 Homework**

---

## 1. The Organization

BlinkSend is a fictional Canadian fintech startup enabling fast, low-cost international money transfers. It operates as a **Money Services Business (MSB)** regulated by **FINTRAC**, with oversight from the Bank of Canada and **FCAC**.

**Employees:** 5 to 8
**Data handled:** full names, email addresses, and bank account details of senders and receivers
**Stage:** early-stage, no dedicated security or compliance hire

---

## 2. Framework Selection

With 5 to 8 employees, ISO 27001 is not the right starting point. It requires external auditors, dedicated resources, and significant investment. Good GRC thinking accounts for organisational capacity, not just risk profile.

The recommended approach is phased:

| Phase | Framework | Timeline | Why |
|---|---|---|---|
| Phase 1 | NIST CSF | Now | Flexible, no certification required, maps to PIPEDA and FINTRAC |
| Phase 2 | CyberSecure Canada | Year 1 to 2 | Canadian government-backed, recognised by insurers and partners |
| Phase 3 | ISO/IEC 27001 | Year 2 to 3 | Global certification target as the company scales |

**Primary framework: NIST CSF**

NIST CSF organises security around five functions: Identify, Protect, Detect, Respond, Recover. It is structured enough to produce real security improvements without requiring a dedicated compliance hire. Its controls map directly onto PIPEDA safeguard obligations and FINTRAC's compliance program requirement.

---

## 3. Business Case

### What Risks It Addresses

- Customer bank details accessed by unauthorised parties
- A breach with no incident response plan in place
- Weak security inherited from third-party payment partners
- A consent checkbox that does not meet PIPEDA's meaningful consent requirement
- No documented compliance program for FINTRAC

### How It Benefits the Organization

- **Risk-aware:** critical assets and threats identified using the NIST CSF Identify function
- **Breach-ready:** documented incident response plan so the team knows what to do
- **Regulation-ready:** FINTRAC and PIPEDA obligations addressed through real controls

### Implementation Priority

1. Access control: limit who can view customer bank details
2. Incident response plan: document what happens if a breach occurs
3. Privacy policy: replace the checkbox with meaningful consent
4. Vendor due diligence: assess third-party payment partners
5. Staff awareness: all 5 to 8 employees understand their responsibilities

---

## 4. Privacy Law Alignment

| Law | Obligation | BlinkSend's Gap |
|---|---|---|
| PIPEDA | Consent, safeguards, breach notification | Checkbox insufficient; no breach response plan |
| Law 25 (Quebec) | Privacy Impact Assessment, Privacy Officer | No privacy governance in place |
| FINTRAC | Documented compliance program | No formal program documented |

---

## Instructor Feedback

Dr. Lloyd Jura noted during office hours that ISO 27001 is too resource-heavy for an early-stage startup with a small team. This submission was updated to reflect that feedback. The phased approach above is a direct response to that conversation.

---

*Completed as part of the SCWIST Cybersecurity Program (2026) | Week 4: Introduction to Cybersecurity Compliance*
*Updated following feedback from Dr. Lloyd Jura, Ph.D., CISSP*
