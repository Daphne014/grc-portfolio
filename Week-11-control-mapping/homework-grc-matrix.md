# Risk, Control, and Evidence Analysis: Mid-Sized Consulting Firm Scenario

## The Scenario in Brief

A 45-person professional services firm runs its operations on Microsoft 365, with staff split between remote and in-office work. The data at stake is not trivial: personal information, financial documents, confidential business records. Security is handled by an outsourced IT provider rather than an in-house team. MFA is live for some accounts but not all of them. Phishing attempts have picked up. Former employee accounts don't always get removed on the schedule they should. And leadership now has two things bearing down on them at once: a client security questionnaire and a compliance review.

Three risks stand out from that picture, and each one traces back to a gap that already shows up in the scenario itself rather than a hypothetical one.

## Risk One: Partial MFA Coverage

The firm's biggest exposure is the gap between "MFA exists" and "MFA is enforced." A control that only covers some of the user base protects some of the data some of the time, which in practice means an attacker only needs to find the accounts still sitting outside that coverage. The fix isn't a new tool; it's closing the gap on the tool already in place, enforced tenant-wide with no exceptions, backed by a recurring access review so coverage doesn't quietly erode again over the next few months.

Proof of this wouldn't be a policy statement. It would be a configuration export showing 100% MFA enrollment across the tenant, plus signed records from each quarterly access review confirming that coverage held.

## Risk Two: Phishing Exposure

Recent concerns already flag rising phishing volume, and a security awareness program that exists on paper isn't the same as one that's actively reducing click-through rates. This risk needs two things working together: ongoing training with simulated phishing tests (not a one-time onboarding module) and email filtering configured at the M365 tenant level to catch what training alone won't.

What proves this is working is training completion data paired with simulation results over time (ideally showing click rates trending down), along with the tenant's email security configuration and any incident logs from filtered or reported phishing attempts.

## Risk Three: Delayed Offboarding

An outsourced IT function without a formal, HR-triggered deactivation process is exactly how former employees keep functional access after they've left. This is a process gap more than a technology gap: the fix is a documented offboarding procedure where account deactivation happens the same day as termination, triggered directly by HR rather than waiting on a support ticket.

Evidence here is straightforward: deactivation logs timestamped against actual termination dates, cross-checked with a signed offboarding checklist for each departure.

## Why This Matters Beyond the Technical Fix

None of these three controls does much for governance or client trust in isolation. MFA blocks unauthorized logins whether or not anyone ever asks about it. What turns a technical safeguard into something a client or auditor can rely on is the documentation trail sitting behind it.

A firm that can produce an MFA configuration report showing full coverage, alongside signed quarterly access reviews, isn't just claiming its data is protected. It's showing that access is managed on purpose, on a schedule, by someone accountable for it. The same is true of offboarding: a same-day deactivation log tied to an HR record demonstrates that a known, common failure point has been closed and is being watched, not assumed away.

That distinction is what a client security questionnaire is actually probing for. Nobody filling one out wants a list of tools the firm owns; they want proof the firm can answer for its own safeguards on demand. A light compliance review works the same way. Controls without evidence are assertions. Controls with evidence are governance, and governance is what a professional services firm is really selling when it asks a client to hand over financial and personal data in the first place.
