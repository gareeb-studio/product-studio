# Product Studio — Governance

*Source: `docs/PRODUCT_STUDIO_HOW_TO_BEGIN.md` (approved version to be recorded in SETUP-001). This file is the working summary; if they conflict, the vote record in `votes/` wins.*

## Golden Rules

1. One active product at a time.
2. Everyone may submit ideas to the Idea Board.
3. Ideas cannot skip phases.
4. Every next phase starts **locked**.
5. Required work/evidence must be completed before a gate vote can open.
6. **Evidence unlocks voting.**
7. **Voting unlocks the next phase.**
8. Voting results and decisions are permanently recorded.
9. Product work must be linked to GitHub Issues/Pull Requests wherever practical.
10. Contributions are measured by approved work, not commit count or lines of code.
11. Voting power, contribution score, and financial ownership are **separate concepts**.
12. Gate requirements cannot be changed during an active vote.
13. A project can be advanced, sent back for rework, paused, or killed.
14. No one pushes directly to the protected production/main branch once development begins.

## Lifecycle & Gates

| Phase | Name | Gate question |
|---|---|---|
| 0 | Idea Board | Is the template complete, problem clear, customer + monetisation + distribution hypotheses present? |
| 1 | Research | Is there enough evidence to spend team time validating this opportunity? |
| 2 | Validation | Has it shown enough real-world potential to justify designing/building an MVP? Validation target must be agreed **before** validation begins. |
| 3 | Product Specification | Vote on the actual plan: scope, non-MVP list, stack, time, budget, roles, Product Captain. Passing authorises development. |
| 4 | MVP Development | All mandatory features done, no blocker bugs, staging build, docs, analytics. Work = Issue → Assign → Branch → PR → Review → Merge → Contribution recorded. Points agreed **before** work starts: XS=1, S=2, M=5, L=8, XL=13. |
| 5 | Testing / QA | Core, edge cases, devices/browsers, auth, payments, security basics, performance, errors, UX, deploy, analytics, backup. Critical blockers must be closed before the launch vote opens. |
| 6 | Launch | Define measurable 30-day targets before launch. After the review period: SCALE / CONTINUE / REWORK-PIVOT / PAUSE / KILL. Only a pass unlocks serious Growth spend. |

Gate decisions: **ADVANCE / REWORK / PAUSE / KILL**.

## Voting Rules

- **Normal phase gate:** at least **2/3 approval** to advance.
- **Major decisions:** **75% approval** — changing ownership, selling the product, outside investment, large unplanned spending, licensing/selling core IP, removing a member from a product, changing fundamental governance rules.
- During an active vote: eligibility is frozen, gate criteria are frozen, votes have a deadline, results stay hidden until voting closes where practical, and every result is permanently recorded in `votes/`.
- Routine decisions do **not** require votes. Phase transitions and major decisions do.

## Three Separate Ledgers

1. **Decision Ledger** (`decisions/` + `votes/`) — gate votes, important decisions, rule changes, budget approvals.
2. **Contribution Ledger** (`CONTRIBUTIONS.md`) — tasks, contributors, approved points, reviews, research, marketing/sales work. Never measured by commits, LOC, messages, hours online, or ideas submitted.
3. **Financial Ledger** (`FINANCE.md`) — member funding, expenses, infrastructure, ads, revenue, refunds, profit, distributions, studio reserve.

**Contribution points do NOT automatically equal ownership or voting power.** Ownership / revenue sharing must be agreed separately and documented before meaningful revenue is involved.

## Co-ownership of the organization

Admitted Studio members are **co-owners** of the GitHub organization (Owner role) —
decided by Baber 2026-10-21, to be ratified in SETUP-001. Admission is therefore an
ownership decision, and the admission threshold (ceil(2/3 x current co-owners)) applies.

## Roles (per active product)

- **Product Captain** — routine product decisions, keeps it moving.
- **Technical Lead** — architecture, engineering quality, deployment, technical reviews.
- **Growth/Marketing Lead** — validation, acquisition, launch, growth experiments.

One person may hold multiple roles in a small team.
