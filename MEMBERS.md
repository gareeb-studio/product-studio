# Members — The Chain

Membership is effective **only** when an admission vote passes AND the PR adding the member here (and to `docs/data/members.json`) is merged. No merge = no membership.

## Co-owner rule (DECIDED by Baber, 2026-10-21 — to be ratified in SETUP-001)

**A person who passes an admission vote is a CO-OWNER, not a plain member.**
On admission they are invited to the GitHub organization with the **Owner** role — equal
technical power over the org and its repos. "Member #N" in the table below is only the
chain order (sequence of admission), not a lower rank.

This means the trust bar for admission votes is an ownership bar: every co-owner can
technically add/remove people and change org settings. The governance ledger — not GitHub
permissions — is what keeps that power inside the voting rules.

## Admission rule (PROPOSED — to be ratified in SETUP-001)

- Member #2: admitted by the Founder alone (1 of 1).
- Member #3 onward: admitted by **at least 2/3 of all current members** (ceil). At 2 members that means both must agree.
- Every voter comments `VOTE: ADMIT` or `VOTE: REJECT` on the applicant's Join Request issue before the deadline.
- The result is permanently recorded in `votes/` as `ADMIT-XXX`.
- A rejected applicant's request is closed and recorded; whether/when they may re-apply is a decision for the current members (not defined in v1 — flag for SETUP-001).

## Current members

| # | Member | GitHub | Role | Admitted by | Date |
|---|---|---|---|---|---|
| 1 | Baber Sheikh | [@b0b90](https://github.com/b0b90) | Founder | Founder — created the Studio | 2026-10-21 |
| 2 | Asad Khilji | [@asadkhilji](https://github.com/asadkhilji) | Co-owner | Baber Sheikh (#1) — founder vote 1/1, Issue #3 | 2026-10-21 |

## Admission history

| Vote | Applicant | Voters | For / Against | Needed | Result | Date |
|---|---|---|---|---|---|---|
| ADMIT-001 | Asad Khilji (@asadkhilji) | Baber Sheikh | 1 / 0 | 1 | PASSED | 2026-10-21 |