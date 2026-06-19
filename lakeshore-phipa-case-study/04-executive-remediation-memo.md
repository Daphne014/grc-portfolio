# Memo: Privacy Risk Review and Recommended Actions
**To:** CEO, Lakeshore Health Technologies
**From:** Compliance & Privacy
**Re:** What a recent Ontario privacy ruling tells us about our own exposure

A clinic in Ontario recently went through a privacy investigation for how it got rid of old patient files. No formal penalty in the end, but only because they fixed everything after the regulator came knocking. The case is worth our attention because the three things the clinic got wrong aren't paper problems. They translate directly to how we handle data.

**What they got wrong, and where we have the same gap.**

They had no written rules for how patient records should be destroyed. Staff worked off a verbal understanding, and when one employee made a different call, there was nothing on paper she was technically breaking. We have the same exposure if our data retention and deletion practices exist only as informal team knowledge rather than documented policy.

Their records were supposed to be shredded. Instead they were torn and put in a bin. The regulator's point wasn't really about shredding versus tearing. It was that nobody was checking whether the right thing was actually happening. If our automated deletion feature removes records from the main database but they're still sitting in backups or a reporting tool, we've made the same mistake in a different format.

It took them over nine months to notify affected patients, partly because they initially convinced themselves nothing had really gone wrong. Under PHIPA s.12(2), the duty to notify kicks in the moment PHI leaves your custody without authorization, not when you've fully confirmed misuse. If our incident response process lets an early "this probably isn't a breach" call go unchallenged, we're set up for the same delay.

**What I'm recommending.**

Get our retention and deletion rules into a formal written policy, not just an understood practice. Before the automated deletion feature launches, confirm it's clearing records from backups and third-party tools, not just the main database. And put basic monitoring on that deletion job so a failure gets caught quickly rather than months down the line.

**The ask.** Two weeks to close the backup and monitoring gaps before the deletion feature goes live. The feature itself is the right move. It just needs those two things in place first.

---
*Grounded in PHIPA Decision 266, IPC, November 22, 2024. Lakeshore Health Technologies is fictional.*
