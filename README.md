# SR Manager — TP² Framework
**Systematic Review App for Neurodivergent Learners in Higher Education**

Researcher: Nae Myo Aung Khing · ESML Doctoral Batch 5 · Chulalongkorn University

🔗 **Live app:** `https://<your-username>.github.io/sr-manager/`

---

## What this is

A self-contained single-file systematic review manager built for the TP² Framework research. Features include:

- Paper library with PRISMA screening (Include / Exclude / Pending)
- Quick Screen mode (keyboard I / X shortcuts)
- DOI auto-fill via CrossRef API
- Evidence panel with variable-level analysis for 16 TP² variables
- Search log with Scopus / ERIC / Google Scholar Boolean strings
- Q1 Scopus journal panel with copy-paste search strings
- Export to CSV, Excel, and backup JSON

## How the library sync works (Option B)

The `papers.json` file in this repo is the **shared library**. When you open the app on any device:

1. It loads your local browser data (localStorage) first
2. Then silently fetches `papers.json` from GitHub and merges any new papers in

To update the shared library after adding papers in the app:
1. Click **☁ papers.json** button in the top toolbar
2. Download the file
3. Replace `papers.json` in this repo with the downloaded file
4. Commit and push → everyone gets the update on next open

## Files

| File | Purpose |
|------|---------|
| `index.html` | The complete SR App (single file, ~365KB) |
| `papers.json` | Shared paper library — update and commit when adding papers |
| `README.md` | This file |

## Updating the app

When a new version of the app is ready:
1. Replace `index.html` with the new version
2. Commit with message like `Update SR App to v7`
3. GitHub Pages deploys automatically within ~60 seconds
