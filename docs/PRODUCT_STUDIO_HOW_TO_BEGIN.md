# Product Studio --- How We Begin

> **Core rule:** Every phase is locked. A project can move to the next
> phase only after the required work is completed and the team passes a
> formal vote.

## 1. Purpose

We are a group of friends who want to turn ideas into real, launched
products using a transparent and fair process.

Our system must make it clear:

-   Who proposed an idea
-   Who researched it
-   Who voted
-   Why a decision was made
-   Who contributed what
-   How much money was contributed or spent
-   What phase the product is currently in
-   What is required before it can move forward

**GitHub will be our source of truth.**

WhatsApp/Discord can be used for conversation, but important ideas,
decisions, work, votes, and contributions must be recorded in GitHub.

------------------------------------------------------------------------

## 2. The Golden Rules

1.  **One active product at a time.**
2.  Everyone may submit ideas to the Idea Board.
3.  Ideas cannot skip phases.
4.  Every next phase starts **locked**.
5.  Required work/evidence must be completed before a gate vote can
    open.
6.  **Evidence unlocks voting.**
7.  **Voting unlocks the next phase.**
8.  Voting results and decisions are permanently recorded.
9.  Product work must be linked to GitHub Issues/Pull Requests wherever
    practical.
10. Contributions are measured by approved work, not commit count or
    lines of code.
11. Voting power, contribution score, and financial ownership are
    separate concepts.
12. Gate requirements cannot be changed during an active vote.
13. A project can be advanced, sent back for rework, paused, or killed.
14. No one pushes directly to the protected production/main branch once
    development begins.

------------------------------------------------------------------------

# 3. Product Lifecycle

``` text
IDEA BOARD
    🔒
    ↓ Gate Vote
IDEA RESEARCH
    🔒
    ↓ Gate Vote
VALIDATION
    🔒
    ↓ Gate Vote
PRODUCT SPECIFICATION
    🔒
    ↓ Gate Vote
MVP DEVELOPMENT
    🔒
    ↓ Gate Vote
TESTING / QA
    🔒
    ↓ Gate Vote
LAUNCH
    🔒
    ↓ Gate Vote
GROWTH / SCALE
```

At every gate, the possible decisions are:

-   **ADVANCE** --- unlock the next phase
-   **REWORK** --- remain in the current phase and fix identified
    problems
-   **PAUSE** --- freeze the product temporarily
-   **KILL** --- stop the product and return to the Idea Board

------------------------------------------------------------------------

# 4. Phase 0 --- Idea Board

This is where we begin.

Every member can submit ideas. Submitting an idea does **not** mean the
team has agreed to build it.

Each idea must contain:

``` text
Idea Name:
Submitted By:
Date:

Problem:
Who has this problem?

Target Customer:
Who exactly would use/pay for it?

Proposed Solution:
What are we proposing to build?

Why Now:
Why is this worth investigating now?

Existing Alternatives:
What are customers using today?

Monetization:
How could it make money?

Distribution:
How could we get our first 100 users?

MVP:
What is the smallest useful version?

Estimated Difficulty:
Small / Medium / Large

Evidence:
Links, screenshots, research, discussions, competitors, etc.
```

Suggested GitHub labels:

``` text
idea
research
voting
validation
approved
rework
paused
killed
building
testing
launched
growth
```

## Gate 0 --- Idea → Research

Before an idea can enter Research:

-   The idea template must be complete.
-   The problem must be understandable.
-   A target customer must be identified.
-   A basic monetization hypothesis must exist.
-   A basic distribution hypothesis must exist.

Then the team votes.

**Recommended rule:** at least 2/3 approval to advance.

------------------------------------------------------------------------

# 5. Phase 1 --- Research

The selected idea is researched before serious work begins.

Required research should include:

-   Problem research
-   Target-user research
-   Competitor analysis
-   Competitor pricing
-   Market demand signals
-   Distribution opportunities
-   Technical feasibility
-   Estimated development effort
-   Expected operating costs
-   Risks
-   Reasons the idea may fail

Research must be attached or linked from GitHub.

## Gate 1 --- Research → Validation

The vote asks:

> **Is there enough evidence to spend team time validating this
> opportunity?**

Possible result:

``` text
ADVANCE
REWORK
PAUSE
KILL
```

Passing unlocks Validation.

------------------------------------------------------------------------

# 6. Phase 2 --- Validation

We test whether real people actually care **before building the full
MVP**.

The validation target must be agreed upon before validation begins.

Possible validation methods:

-   Customer interviews
-   Landing page
-   Waitlist
-   Prototype
-   Pre-orders
-   Demo
-   Ads
-   Outreach
-   App-store/search research
-   Direct sales conversations

Example success criteria:

``` text
10 customer interviews
AND
3 people willing to pay
```

or:

``` text
100 qualified landing-page signups
```

The exact target depends on the product.

## Gate 2 --- Validation → Product Specification

The team reviews the evidence.

The vote asks:

> **Has the idea shown enough real-world potential to justify designing
> and building an MVP?**

If it fails, the team may rework, pause, or kill it.

------------------------------------------------------------------------

# 7. Phase 3 --- Product Specification

No major development begins until the MVP is defined.

Create:

-   Product objective
-   Target user
-   Core user journey
-   MVP feature list
-   Explicit non-MVP list
-   Technical architecture
-   Technology stack
-   UI/UX direction
-   Database/API requirements
-   Security/privacy requirements
-   Analytics requirements
-   Deployment plan
-   Estimated development time
-   Estimated costs
-   Team responsibilities
-   Product Captain

Example:

``` text
MVP

✓ Registration
✓ Login
✓ Core product feature
✓ Payments
✓ Basic analytics
✓ User settings

NOT MVP

✗ Team accounts
✗ Public API
✗ Mobile application
✗ Advanced reporting
```

## Gate 3 --- Specification → Development

The team votes on the **actual plan**, including expected time and
budget.

Example:

``` text
Estimated work: 180 hours
Server/API budget: $150
Marketing preparation: $100
Target MVP date: 30 November
```

Passing this vote officially authorizes development.

------------------------------------------------------------------------

# 8. Phase 4 --- MVP Development

The specification is converted into GitHub Issues.

Example:

``` text
#101 Google Authentication — 3 points
#102 User Dashboard — 5 points
#103 Payment Integration — 8 points
#104 Core Generator — 13 points
```

Workflow:

``` text
Issue
  ↓
Assignment
  ↓
Branch
  ↓
Development
  ↓
Pull Request
  ↓
Review
  ↓
Merge
  ↓
Contribution Recorded
```

Task points should normally be agreed **before work starts**.

Suggested sizing:

``` text
XS = 1
S  = 2
M  = 5
L  = 8
XL = 13
```

## Gate 4 --- Development → QA

Minimum requirements might include:

-   All mandatory MVP features completed
-   No known blocker bugs
-   Deployment/staging build available
-   Basic documentation complete
-   Analytics implemented
-   Required accounts/configuration documented

The team then votes to enter formal QA.

------------------------------------------------------------------------

# 9. Phase 5 --- Testing / QA

Test:

-   Core functionality
-   Edge cases
-   Different devices/browsers where relevant
-   Authentication
-   Payments
-   Security basics
-   Performance
-   Error handling
-   User experience
-   Installation/deployment
-   Analytics
-   Backup/recovery where relevant

Bugs become GitHub Issues.

Critical launch blockers must be closed before a launch vote can open.

## Gate 5 --- QA → Launch

The vote asks:

> **Are we willing to put our name behind this product and release it to
> real users?**

Passing authorizes launch.

------------------------------------------------------------------------

# 10. Phase 6 --- Launch

Launch activities may include:

-   Production deployment
-   Domain
-   App stores
-   Product Hunt
-   Social media
-   Communities
-   Direct outreach
-   SEO/ASO
-   Paid acquisition
-   Existing network
-   Email
-   Partnerships

Before launch, define measurable targets.

Example:

``` text
First 30 Days

100 registrations
20 active users
5 paying customers
$100 MRR
<5% critical failure rate
```

## Gate 6 --- Launch → Growth

After the agreed review period, the team evaluates actual results.

Vote:

``` text
SCALE
CONTINUE
REWORK / PIVOT
PAUSE
KILL
```

Only a passing vote unlocks serious Growth/Scale investment.

------------------------------------------------------------------------

# 11. Voting Rules

Initial recommended rules:

### Normal Phase Gate

**2/3 approval required.**

### Major Decisions

Require **75% approval** for matters such as:

-   Changing ownership
-   Selling the product
-   Taking outside investment
-   Large unplanned spending
-   Licensing/selling core IP
-   Removing a member from a product
-   Changing fundamental governance rules

### Voting Integrity

During an active vote:

-   Eligibility is frozen.
-   Gate criteria are frozen.
-   Votes have a deadline.
-   Results should preferably remain hidden until voting closes.
-   Every result is permanently recorded.

Example record:

``` text
GATE-003

Transition:
Validation → Product Specification

Requested by:
Baber

Eligible voters:
5

Votes cast:
5

Advance: 4
Rework: 1
Pause: 0
Kill: 0

Required:
66.67%

Result:
PASSED

Date:
2026-10-21
```

------------------------------------------------------------------------

# 12. Contribution Tracking

Do **not** measure contribution using:

-   Number of commits
-   Lines of code
-   Number of messages
-   Hours online
-   Number of ideas submitted

Track completed, accepted work.

Contribution categories:

``` text
Idea / Research
Product
Development
Design
Testing / QA
Marketing
Sales
Operations
Capital
```

Example:

  --------------------------------------------------------------------------------------
  Member     Research   Product      Dev   Design       QA   Marketing    Sales    Total
  -------- ---------- --------- -------- -------- -------- ----------- -------- --------
  Member A         18        20       61        0       12          10        0      121

  Member B         22        14       28       20       16           8        0      108

  Member C         13         7        4        5        9          43       30      111
  --------------------------------------------------------------------------------------

The contribution dashboard should link points back to the work that
generated them.

------------------------------------------------------------------------

# 13. Three Separate Ledgers

We maintain three independent records.

## Decision Ledger

Records:

-   Gate votes
-   Important decisions
-   Rule changes
-   Budget approvals

## Contribution Ledger

Records:

-   Tasks
-   Contributors
-   Approved points
-   Reviews
-   Research
-   Marketing/sales work

## Financial Ledger

Records:

-   Member funding
-   Product expenses
-   Infrastructure
-   Advertising
-   Revenue
-   Refunds
-   Profit
-   Distributions
-   Studio reserve

**Contribution points do not automatically equal ownership or voting
power.**

Ownership/revenue sharing must be agreed separately and documented
before meaningful revenue is involved.

------------------------------------------------------------------------

# 14. Roles

For each active product assign:

### Product Captain

Responsible for routine product decisions and keeping the project
moving.

### Technical Lead

Responsible for architecture, engineering quality, deployment, and
technical reviews.

### Growth/Marketing Lead

Responsible for validation, acquisition, launch, and growth experiments.

One person may hold multiple roles in a small team.

Routine decisions do not require votes. **Phase transitions and major
decisions do.**

------------------------------------------------------------------------

# 15. Repository Structure

Start with one central repository:

``` text
product-studio/
│
├── README.md
│
├── GOVERNANCE.md
│
├── CONTRIBUTIONS.md
│
├── FINANCE.md
│
├── ideas/
│   └── README.md
│
├── products/
│   └── active-product.md
│
├── decisions/
│   └── README.md
│
├── votes/
│   └── README.md
│
└── .github/
    └── ISSUE_TEMPLATE/
```

As soon as an idea becomes a real software product, its source code can
live in its own product repository while the central repository remains
the governance headquarters.

------------------------------------------------------------------------

# 16. How We Begin --- Day 1

Do **not** start by building the dashboard software.

Start the process manually and automate it after the rules have been
tested.

### Step 1 --- Create GitHub Organization

Create one organization owned/administered appropriately for the group.

### Step 2 --- Create `product-studio` Repository

This becomes the headquarters.

### Step 3 --- Add Every Member

Every member uses their own GitHub account so activity is attributable.

### Step 4 --- Approve Governance

Before submitting ideas, everyone reviews and approves this document.

Any disagreements about voting, contributions, ownership, spending, or
decision-making should be resolved **before product development**.

### Step 5 --- Open the Idea Board

Every member submits ideas using the same template.

### Step 6 --- Set Submission Deadline

Example:

``` text
Idea submission opens: Monday
Idea submission closes: Sunday
```

### Step 7 --- Review Ideas

Discuss, challenge assumptions, add evidence, and identify duplicates.

### Step 8 --- Hold Gate 0 Vote

Select which ideas deserve deeper research.

If several survive, research them and use the later gate to select the
strongest opportunity.

### Step 9 --- Select ONE Active Idea

Once the final idea passes into the active pipeline:

> **No second product becomes active until the current product is
> launched, paused, or killed through the formal process.**

### Step 10 --- Start Contribution Tracking

From the first research task onward, accepted work is recorded against
the member who completed it.

------------------------------------------------------------------------

# 17. What We Should Automate Later

After we have used the manual system and understand our actual needs,
automate:

-   Idea submission
-   Idea board
-   Gate status
-   Voting
-   Hidden vote results
-   Vote deadlines
-   Phase locking
-   Checklist enforcement
-   GitHub activity collection
-   Contribution scoring
-   Contribution graphs
-   Decision history
-   Product progress
-   Financial dashboard
-   Notifications
-   Member profiles

Eventually the dashboard could show:

``` text
ACTIVE PRODUCT
────────────────────────
Product X

Current Phase:
VALIDATION

Progress:
██████████████░░ 78%

NEXT GATE
🔒 Validation → Specification

Checklist:
✓ Customer interviews
✓ Competitor analysis
✓ Pricing test
✗ Minimum validation target

Vote:
LOCKED


TEAM CONTRIBUTION
────────────────────────
Member A  █████████████ 121
Member C  ████████████  111
Member B  ███████████   108
```

------------------------------------------------------------------------

# 18. Our Operating Principle

> **Ideas are cheap. Evidence earns attention.**
>
> **Evidence unlocks the vote.**
>
> **Voting unlocks the next phase.**
>
> **Approved work creates contribution.**
>
> **GitHub preserves the history.**
>
> **Only one product receives the team's active focus at a time.**

------------------------------------------------------------------------

## First Action

Create the GitHub organization and the `product-studio` repository.

Then create the first GitHub Issue:

``` text
SETUP-001 — Approve Product Studio Governance

Goal:
All founding members review and approve the initial operating rules.

Required before completion:
□ Voting threshold agreed
□ Gate system agreed
□ Contribution system agreed
□ Financial tracking agreed
□ Product ownership principle agreed
□ Member roles agreed
□ All founding members approve

Until SETUP-001 passes:

🔒 IDEA SUBMISSION IS NOT YET OPEN
```

**The first thing your team votes on should not be a product idea.\
The first vote should be the rules by which every future product will be
selected and built.**
