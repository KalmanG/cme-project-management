# Notes for AI Agents

This file is the single place AI agents should read before picking up work in this repo. Keep it short and accurate — append session entries at the bottom rather than rewriting.

## What this repo is (and isn't)

- **Is:** a lightweight issue tracker feeding the [CME First Board](https://github.com/users/KalmanG/projects/1) GitHub Project. It holds non-code work: milestones, JDs, market-research tasks, operating-agreement notes.
- **Isn't:** the CME Wizard application codebase. Issues like "Grouping implementation," "Pricing implementation," "Work on LMS," and other implementation tasks refer to a CME Wizard codebase that lives elsewhere. Don't try to "implement" them here — they'll stay as tracking issues until the CME Wizard repo is linked.

## Where work gets committed

- **Hiring / JDs →** `docs/hiring/` (e.g., `associate-marketer.md`)
- **Operating-agreement drafts →** `docs/legal/` (create when needed)
- **Market-research outputs →** `docs/research/` (create when needed)

Always commit on a branch and open a PR. Never push to `main` directly.

## Known issue-backlog hygiene

Several issues are empty-body duplicates of richer ones. Previously flagged:

| Empty dup | Canonical issue |
|---|---|
| #12 | #5 (stop notice) |
| #13 | #4 (other enrichment) |
| #14 | #3 (people field) |
| #15 | #2 (grouping — sub-task of grouping + pricing) |
| #16 | #2 (pricing — sub-task of grouping + pricing) |

If a maintainer hasn't closed them, leave them alone — don't re-comment.

## Known blockers

- **#22 Operating agreement paragraph:** requires a Google Doc (`docs.google.com/document/d/1YyPB02ZTUfTLZRX7jxCMOL24jZ3z4AIsUDXi6OPAmbk`). An agent without Google auth can't open it. If you're picking this up, ask the user to paste the surrounding context into the issue first.

## Session log

Append new entries at the bottom. Format: date, what shipped, what was blocked, what future agents should know.

### 2026-04-20 — Claude (Opus 4.7)

**Shipped**
- PR #23 — drafted `docs/hiring/associate-marketer.md` closing #19 and #20. JD covers all acceptance-criteria bullets; left placeholders for comp range and apply-to email that a human should confirm before posting.
- Triage comments on #12, #13, #14, #15, #16 recommending closure as duplicates of their richer counterparts.
- Triage comment on #22 documenting the Google Doc blocker.
- Created this `AGENTS.md` as the onboarding note for future agents.

**Tried and ruled out**
- Implementing #2 / #6 / #11 / #15 / #16 — these are CME Wizard application work. No CME Wizard codebase is reachable from this repo; the working directory the session ran in was a Viv WordPress install unrelated to CME Wizard.
- Acting on #22 — blocked on Google Doc access as described above.
- Acting on #21 — network-research task owned by a specific person (Gabor), not an agent task.

**Future-agent suggestions**
- When the CME Wizard repo gets linked, add a pointer from this file so agents know where to cut implementation PRs.
- The market-research issues (#8–#11) are gated on the May 15, 2026 CME Wizard launch. Don't start them before then.
