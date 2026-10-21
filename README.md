# Open Bounties

**Monetize open-source contributions via direct payments and bounties.**

A live bounty board web app: maintainers post bounties on real issues and features, contributors claim them, submit work, and get tracked to payout. Keyless v1 — all data persists in the browser via localStorage, no API keys or backend required.

**Live:** not deployed yet — open `index.html` in a browser, or host it as a static site.

## Features

- **Post bounties** — title, repo link, amount (USD), description with acceptance criteria
- **Browse & filter** — search by title/repo/description, filter by status (Open / Claimed / In review / Completed / Paid out), sort by newest or highest amount
- **Claim a bounty** — assign yourself by handle; status moves to Claimed
- **Submit work** — link your PR/commit with notes; status moves to In review
- **Mark complete** — payout flagged as **"pending owner approval"** (internal accounting only — this app never moves real money)
- **Confirm payout** — owner confirms the off-platform payment, status moves to Paid out
- **Activity timeline** per bounty + JSON export of all data
- Seeded with 4 example bounties covering every status

## Tech

Single self-contained `index.html` (HTML + CSS + JS, zero dependencies). Deploys as a static site.

## Payouts

All payout tracking is internal accounting only. The board never sends real payments — when work is marked complete, the payout shows "pending owner approval" and the poster settles it off-platform.
