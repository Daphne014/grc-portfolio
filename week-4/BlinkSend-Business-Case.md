# BlinkSend: Framework Selection & Business Case
**SCWIST Cybersecurity Program | Week 4 Homework**

---

## 1. The Organization

BlinkSend is a fictional Canadian fintech startup that enables individuals to send and receive money globally, quickly, and at competitive exchange rates. Speed is its core promise: transfers happen in the blink of an eye.

It operates as a Money Services Business (MSB) regulated by **FINTRAC**, with additional oversight from the Bank of Canada and the **Financial Consumer Agency of Canada (FCAC)**. Customers are individuals in Canada sending money to recipients globally.

**Data handled:** full names, email addresses, and bank account details of senders and receivers.
**Stage:** early-stage startup with limited internal security infrastructure.

---

## 2. Most Appropriate Framework: ISO/IEC 27001

ISO/IEC 27001 is the right fit for BlinkSend. It is an international standard for managing information security, recognized in over 150 countries, and one of the few frameworks that offers formal certification.

**Why not the others?**

| Framework | Reason Not Selected |
|---|---|
| NIST CSF | U.S.-centric, no certification pathway |
| CyberSecure Canada | Designed for domestic SMEs, limited international recognition |
| COBIT | Better suited to larger, more mature organizations |

BlinkSend operates globally from day one. It needs a framework that global partners actually recognize, and ISO 27001 is the one they ask for by name.

---

## 3. Business Case

### Why This Framework Fits

BlinkSend handles some of the most sensitive data that exists: bank details and financial transactions. From day one, it needs to show customers, partners, and regulators that it takes that seriously.

ISO 27001 covers people, processes, and technology together. Its controls map directly onto **PIPEDA** and **Law 25** requirements around consent, data safeguards, vendor risk, and breach notification. It also gives BlinkSend something concrete to show partners: a certification, not just a promise.

---

### What Risks It Addresses

BlinkSend's biggest risks right now are straightforward:

- Customer bank details could be accessed by someone who should not have them
- A breach could happen with no plan for what to do next
- A third-party payment partner could have weak security that BlinkSend inherits
- The current consent mechanism (a single checkbox confirming the user knows their recipient) does not tell customers how their data is actually being used or protected

These are not hypothetical. They are the exact gaps regulators look for and that fraud actors look to exploit.

---

### How It Benefits the Organization

Three things change after ISO 27001 implementation:

1. **Audit-ready.** Regulators and partners can see documented controls, not just good intentions.
2. **Partner-ready.** Global payment institutions routinely require ISO 27001 before signing agreements. Certification removes that barrier early.
3. **Breach-ready.** Not in the sense that breaches become impossible, but that the company knows what to do if one happens. That is what compliance actually means.

---

## Implementation Considerations

Certification is a 12 to 18 month phased commitment, which is realistic for an early-stage startup working within budget constraints. BlinkSend can prioritize the highest-risk controls first and work toward full certification progressively.

As the business scales into new markets, additional data protection requirements will apply depending on where recipients are located. Building legal guidance on key jurisdictions into the growth plan early keeps compliance ahead of the business rather than behind it.

---

## Privacy Law Alignment

| Law | Obligation | BlinkSend's Gap |
|---|---|---|
| PIPEDA | Meaningful consent, data safeguards, breach notification | Consent checkbox is insufficient; no breach response plan |
| Law 25 (Quebec) | Privacy Impact Assessment, designated Privacy Officer, right to erasure | No privacy governance structure in place |
| FINTRAC | Documented compliance program for MSBs | No formal program documented |

ISO 27001 implementation directly produces the policies, controls, and documentation these obligations require.

---

*Completed as part of the SCWIST Cybersecurity Program (2026) | Week 4: Introduction to Cybersecurity Compliance*
