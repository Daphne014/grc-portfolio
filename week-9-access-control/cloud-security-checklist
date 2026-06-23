# Access Control & Cloud Security Checklist: Lakeshore Health Technologies

## Overview

This checklist sets out baseline identity, cloud access, monitoring, and shadow IT controls for a mid-size organization handling sensitive data. It is built against Lakeshore Health Technologies, a fictional Ontario health technology company operating under PHIPA, and reflects the access control failures most commonly cited in IPC decisions and cloud misconfiguration breaches.

## Scenario / Context

Lakeshore Health Technologies stores patient records in cloud infrastructure and relies on a mix of in-house systems and third-party SaaS tools. Under the shared responsibility model, the cloud provider secures the underlying infrastructure, but Lakeshore remains responsible for configuring access, managing identities, and securing the data it puts into that infrastructure. Misconfigured storage permissions, unreviewed access rights, and unsanctioned tooling are the three most common entry points for unauthorized disclosure under PHIPA, and all three sit on Lakeshore's side of that line. The checklist below maps each control to the risk it closes and the prevention approach an auditor would expect to see evidenced.

## Checklist

| Control | Risk Addressed | Prevention |
|---|---|---|
| Multi-factor authentication (MFA) | Credential compromise, account takeover. | Enforce on all admin and remote access accounts; no legacy exceptions. |
| Least-privilege access | Excessive privilege, lateral movement after compromise. | RBAC tied to job function, reviewed at onboarding and role change. |
| Periodic access review | Orphaned accounts, privilege creep. | Quarterly recertification, signed off by data owners. |
| Default-deny cloud storage | Misconfigured storage exposing sensitive files. | CSPM tooling flagging public-facing storage automatically. |
| Centralized logging and alerting | Breaches going undetected. | SIEM or cloud-native logging with anomaly thresholds. |
| Shadow IT inventory | Unapproved tools bypassing security controls. | Discovery scans paired with an approved-vendor list. |
| Orphaned account deprovisioning | Stale credentials, unauthorized access. | Automated deprovisioning tied to HR offboarding. |
| Shared account elimination | Loss of accountability for individual actions. | Migrate to individual accounts with PAM. |
| Shared responsibility documentation | Coverage gaps where both sides assume the other owns a control. | Responsibility matrix per cloud service, reviewed at renewal. |

## Key Takeaways / Recommendations

Organizations operating under PHIPA should treat access control as a continuous program, not a one-time configuration. A default-deny posture on cloud storage closes the most common exposure path seen in breach decisions, but it only holds if paired with scheduled access reviews and logging that someone actually monitors. Shadow IT cannot be controlled through policy alone; it requires active discovery, because unsanctioned tools will not show up in a self-reported audit.

## Frameworks Referenced

- PHIPA (safeguard requirements, ss. 12-13)
- NIST CSF 2.0 (Protect, Detect functions)
- ISO 27001:2022 Annex A (access control, A.5 and A.8 series)
- OPC guidance on cloud computing and third-party risk
