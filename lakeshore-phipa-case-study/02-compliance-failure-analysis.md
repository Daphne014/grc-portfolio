# Compliance Failure Analysis
**Lakeshore Health Technologies | GRC Compliance Project | Daphne Obadan**

PHIPA Decision 266 found a clinic that had been disposing of patient records by hand-tearing them, leaving them in a recycling bin, and letting cleaners take them to a public dumpster. Then waited nine months to tell the 482 patients affected. Each legal failure is mapped below to what that same gap looks like inside Lakeshore, a fictional cloud platform handling PHI for GTA clinics.

| Section | What the law requires | What the clinic did | Lakeshore's version of the same risk |
|---|---|---|---|
| s.10(1), s.10(2) | Written policies on how PHI is handled, and actually following them | No written policy existed; only verbal expectations | Retention or access rules that live in one engineer's head, never written down |
| s.12(1) | Reasonable safeguards against PHI being lost, stolen, or disclosed without authority | No oversight of how disposal actually happened | Database access with no logging on who queried or exported PHI |
| s.13(1) | PHI must be disposed of securely and irreversibly | Torn but readable records reached a public dumpster | Data deleted from the main system but still sitting in backups or a third-party tool |
| s.12(2) | Notify affected individuals at the first reasonable opportunity | 9+ month delay; initially argued it wasn't even a breach | Incident response stalled by an early internal call that "this probably isn't a breach" |

**s.10(1) and s.10(2), Information Practices.** The clinic had nothing in writing. When the office manager started tearing records instead of shredding them, there was no documented standard she was actually breaking. That's the legal problem, not just an operational one. Without written policies, there's nothing enforceable. Lakeshore's version of this isn't about paper, it's about undocumented deletion schedules, informal access rules, or processes that only one person actually understands. No written standard means no real standard.

**s.12(1), Security.** The IPC has been clear across multiple decisions that meeting the "reasonable steps" standard under s.12(1) requires administrative and technical safeguards working together, not just good intentions. The clinic had a verbal instruction to shred records. Nobody was checking whether that instruction was followed. One employee made an unsupervised call and nothing caught it. For Lakeshore, the equivalent is a developer with standing production access and no audit log on what they touched. Different mechanism, same missing oversight layer.

**s.13(1), Handling of Records.** The IPC investigator actually pieced the torn records back together during the investigation and could read patient names, dates of birth, and clinical notes from the fragments. Torn isn't destroyed. For Lakeshore, the parallel is a record deleted from the primary database that's still fully recoverable from a 90-day backup or still sitting in a third-party analytics feed. Looks deleted. Isn't actually gone.

**s.12(2), Notification.** This one's worth slowing down on, because the nine-month delay wasn't mainly a paperwork problem. The clinic initially decided internally that what happened wasn't a breach at all, since it believed the source had returned all affected records to the IPC. That assumption went unchallenged for months. The IPC disagreed, finding that PHI had left the clinic's custody and control without authorization, which triggers the notification duty under s.12(2) regardless of whether anyone actually misused the information. Lakeshore could have a notification template ready to send in 24 hours and still hit the same delay if nobody is willing to make the call that a breach has occurred.

---
*Sourced from the publicly available text of PHIPA Decision 266, IPC, November 22, 2024, and the relevant sections of PHIPA. Lakeshore Health Technologies is fictional.*
