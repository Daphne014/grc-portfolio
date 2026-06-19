# Privacy Impact Assessment
**Lakeshore Health Technologies | GRC Compliance Project | Daphne Obadan**

After PHIPA Decision 266 flagged how easily manual disposal decisions can go wrong, Lakeshore is building an automated PHI disposal feature. Once a patient record passes its legally defined retention period, the system deletes it automatically. No staff member makes that call. This PIA assesses what risks the automation itself might introduce before it goes live.

**What data is involved.** Full patient records held on behalf of Lakeshore's clinic clients: names, dates of birth, contact details, treatment history, clinical notes. The feature also creates a deletion log recording when each record was removed and which retention rule triggered it.

**How it works.** A nightly job checks each record against its retention period. Anything past its deadline gets deleted from the primary production database. The deletion currently doesn't extend to backup snapshots, which run on a 90-day rolling cycle, or to the third-party analytics tool that receives a daily data feed of active records.

**The risks worth flagging.**

The nightly schedule means a record that crosses its retention deadline at any point during the day stays in the live system, fully accessible, for up to 24 hours past its legal cutoff. It's a smaller version of the anchor case, PHI existing past the point where Lakeshore is legally permitted to keep it. Lower severity, but the same kind of failure under s.13(1).

The backup and analytics gap is the bigger concern. Deleting from the primary database doesn't mean the record is gone if it's still sitting in backups for 90 days or in a third-party tool indefinitely. The IPC was explicit in Decision 266 that disposal under s.13(1) means irreversible destruction, not just removal from the main system. This is the digital equivalent of tearing records instead of shredding them.

If the nightly job fails silently, with no alert sent to anyone, expired records could pile up in the live system with nobody noticing. The clinic in the anchor case didn't realize records had left its control until an external party raised it. An unmonitored automated system can recreate that exact blind spot.

| Risk | Severity | Fix required before launch |
|---|---|---|
| 24-hour window before deletion runs | Low | Restrict access to record immediately on retention expiry |
| Records persist in backups and analytics feed | High | Extend deletion to all systems; verify and log each purge |
| Silent job failure with no alert | Medium | Active failure monitoring to a named owner |

**Recommendation: Approve with conditions.** The automation is the right response to what went wrong in the anchor case. Removing human judgment from the disposal process directly addresses the s.13(1) failure. It shouldn't go live until the backup and analytics gap is resolved and failure monitoring is in place. The 24-hour access window is a lower-priority fix and can be tracked as a documented follow-up item.

---
*Built on the regulatory reasoning in PHIPA Decision 266, IPC, November 22, 2024. Lakeshore Health Technologies is fictional.*
