# Voice Agents QA Dashboard

An internal quality assurance dashboard for the EvenUp Voice Agents team. Built as a single self-contained HTML file — no backend, no installation required.

**Live URL:** https://annchenlr.github.io/qa-dashboard/

---

## What It Does

Manages the end-to-end QA workflow for AI voice agent calls:

- Ingests tickets from Airtable (via Zapier)
- Auto-assigns tickets to reviewers by priority tier
- Provides a structured scorecard for each call type
- Writes scores, QA results, and dispositions back to Airtable
- Generates weekly reports with Slack-ready summaries

---

## Priority Tiers

| Tier | Behavior |
|---|---|
| HP (High Priority) | Auto-assigned immediately during business hours |
| T1 (Tier 1) | Released in waves at 3:00, 4:00, and 4:30 PM EST |
| PLAAS | Discretionary — manually assigned or skipped at EOD |
| T2 / Other | Auto-skipped, never enter the active queue |

---

## Getting Started

1. Open the live URL above in Chrome, Edge, or Safari
2. Enter your Airtable personal access token when prompted
3. Select your name as the active reviewer
4. Start working your queue

**First time setup:** See the [Team Onboarding Guide](ONBOARDING.md) for step-by-step instructions including how to create your Airtable token.

---

## Updating the Dashboard

When a new version is released:

1. Download the new `qa-queue-dashboard.html` file
2. Rename it to `index.html`
3. Go to this repo → **Add file** → **Upload files**
4. Upload `index.html` — it will overwrite the existing version
5. Commit changes — the live URL updates automatically within 1-2 minutes

---

## Tech Stack

- **Frontend:** Vanilla HTML/CSS/JavaScript (single file, no dependencies)
- **Data:** Airtable REST API
- **Hosting:** GitHub Pages
- **Automation:** Zapier (ticket ingest)

---

## Repo Structure

```
index.html        ← The dashboard (this is what runs at the live URL)
README.md         ← This file
```

---

## Contact

For access or issues, contact **Ann Chen** or your team lead.
