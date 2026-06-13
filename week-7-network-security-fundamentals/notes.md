# Week 7: Network Security Fundamentals for GRC

**SCWIST Cybersecurity Scholars Program | June 2026**
**Stream:** Cybersecurity (Virtual) | **Instructor:** Brian Marshall

---

## What This Week Covered

Network security from a GRC lens: reading network diagrams, identifying missing controls, and translating technical risk into plain language for audits and stakeholder conversations.

---

## Key Concepts

**Firewalls.** In most real environments, one device handles routing, firewall filtering, VPN, and logging all at once. The GRC concern is not whether a firewall exists; it is whether someone is reviewing the rules, how often, and what the change approval process looks like.

**Cloud networks.** A cloud network works like a building. The whole building is called a VPC (Virtual Private Cloud): the private space a company owns in the cloud. Inside, subnets are the individual rooms. They keep systems separated so that a problem in one area does not spread to everything else.

Within those rooms, access is controlled in two ways. A Network ACL is a fixed rule list applied to an entire subnet: it decides what traffic is allowed in or out at the room level. A Security Group is attached to a single system or resource: it is more precise and automatically allows expected reply traffic through without needing a separate rule for it.

The GRC risk in cloud environments is not usually a misconfigured rule. It is accountability. Security groups are typically set up by product development teams, not a central security function. Organisations end up with hundreds of them, no documented owner, and no review cycle. Accountability for the controls has quietly disappeared.

**VPNs and Zero Trust.** A VPN creates an encrypted tunnel between a user and a corporate network. It protects data in transit. It does not verify whether the connecting device is safe, does not restrict what the user can access once inside, and will not stop malware already on the device from entering the environment. Zero Trust addresses this gap by removing the assumption that being inside the network means being trusted. Every access request is verified independently, and access is limited to only what is needed for that specific role or task.

---

## Risk Register Entry

**Scenario:** Cloud environment where security group rules have not been reviewed in over 12 months and no owner is documented.

| Field | Detail |
|-------|--------|
| Asset | Cloud-hosted database containing customer PII |
| Threat | Unauthorized access; lateral movement between systems |
| Vulnerability | Security groups have no assigned owner and have not been reviewed |
| Likelihood | High |
| Impact | High: regulatory exposure, reputational damage |
| Control Recommendation | Assign documented owners; quarterly review cycle; least privilege applied per group |

---

## Audit Findings and What They Mean

**Firewall rules have no documented owner.**
A named individual or team should be responsible for each rule set, recorded in a policy or asset register. Without this, no one is accountable when rules become outdated or misconfigured.

**No formal change control process for rule modifications.**
Changes to firewall or security group rules should be requested, reviewed, approved, and logged. Undocumented changes cannot be audited or reversed reliably.

**Security groups have not been reviewed and the total count is unknown.**
If an organisation cannot state how many security groups exist or when they were last reviewed, that is a finding in itself. Scale without oversight is a control gap.

**No segmentation between sensitive and non-sensitive systems.**
Sensitive data should sit in its own network zone. A flat network, where all systems can communicate freely, means one breach can reach everything.

**VPN access is not monitored after authentication.**
Getting through the VPN is only the first step. Activity inside the network should be logged and reviewed separately from the authentication event.

**Access model does not align with Zero Trust.**
If users receive broad network access simply by connecting, the organisation is still operating on a trust-by-location model. Zero Trust requires verifying access per request and scoping it to what is specifically needed.

---

*Part of the SCWIST 2026 Skills for Success Cybersecurity Scholars Program. All scenarios represent academic exercises for portfolio development.*
