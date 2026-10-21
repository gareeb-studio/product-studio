# PROPOSAL — Chain Admission (for the SETUP-001 vote, NOT yet a rule)

Status: **Proposed by Baber, 2026-10-21. Not approved.** It becomes a rule only if SETUP-001 / a governance vote records it.

## The idea (Baber's words, paraphrased)
A public webpage (GitHub Pages) with a shareable link. Friends open it, join with their GitHub account, and entry is by vote that grows like a chain:

- Baber lets in Member #2.
- Baber + Member #2 let in Member #3.
- Baber + #2 + #3 let in Member #4 — and so on.

## How it maps onto the existing rules (no new math needed)
Admission threshold = the normal gate threshold: **ceil(2/3 × current members)**.

| Current members | ADMIT votes needed | Effect |
|---|---|---|
| 1 | 1 | Founder alone admits #2 |
| 2 | 2 | Both must agree for #3 — one no blocks |
| 3 | 2 | |
| 4 | 3 | |
| 5 | 4 | |
| 6 | 4 | |

## How "Join with GitHub" works in v1 (no backend, $0)
1. The Pages site (`docs/index.html`) has one config line: `REPO`.
2. "Join with GitHub" opens a pre-filled Join Request **issue** in the repo. The applicant must be signed into GitHub, and the issue author *is* their verified GitHub identity — GitHub does the authentication for us.
3. Members vote in issue comments (`VOTE: ADMIT` / `VOTE: REJECT`) — permanently recorded, attributable, free.
4. On a pass, a PR adds the applicant to `MEMBERS.md` + `docs/data/members.json` + a record in `votes/`. **Merge = membership.** The site reads `members.json`, so the page updates itself.

## What v1 deliberately does NOT do
- No in-page OAuth login button that writes data. A true OAuth login needs a GitHub OAuth App + a tiny server/worker to hold the client secret (a secret can never live in a static page). That is v2, buildable later on a free Cloudflare Worker — only worth it if issue-voting ever feels clunky.
- No automated vote counting in v1. Counting 2–6 comments by hand is trivial; automate after the manual process has been used (§17 of the source doc).

## To publish the page
After the repo exists on GitHub: Settings → Pages → Source: Deploy from a branch → Branch: `main`, folder: `/docs`. Share the resulting `https://<org>.github.io/product-studio/` link (e.g. on WhatsApp). The repo itself can stay public for the page + issues while product code later lives in separate private repos — decide public/private in SETUP-001 (flag: a private repo cannot host a free Pages site on the free plan, and join issues need the applicant to be able to open them).
