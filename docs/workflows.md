# Workflows

GitHub Actions workflows in this repo and how to use them.

---

## Weekly meeting issue

**File:** `.github/workflows/weekly-meeting-issue.yml`

**What it does:** Every **Monday 9:00 UTC** (and on manual run), creates a new issue with the [Meeting](../.github/ISSUE_TEMPLATE/meeting.md) template and posts a comment that tags contributors and asks them to post progress and questions before the meeting (no questions = no air time).

**Inputs:** None (scheduled) or trigger manually from **Actions → Weekly meeting issue → Run workflow**.

**Setup:**
- Add GitHub usernames to [`.github/meeting-contributors.txt`](../.github/meeting-contributors.txt) (one per line, with or without `@`). Those users are @-mentioned in the comment.

---

## Weekly sync agenda

**File:** `.github/workflows/weekly-sync-agenda.yml`

**What it does:** Runs **Monday 16:00 UTC** (and on manual run). Finds the open weekly sync issue (created that morning), sends **all comments** to OpenRouter (**google/gemini-2.5-flash-lite**), and asks the model to extract **discussion points** (topics that need air time). It then **edits the issue body** and replaces the “### Agenda” section with that list. Bot comments are skipped.

**Inputs:** None (scheduled) or trigger manually from **Actions → Weekly sync agenda → Run workflow**.

**Setup:** Same as Google Doc → Meeting notes: **OPENROUTER_API_KEY** repo secret (see above).

---

## Google Doc → Meeting notes

**File:** `.github/workflows/google-doc-to-meeting-notes.yml`

**What it does:** Fetches a **public** Google Doc (with Summary and Transcript sections), sends it to OpenRouter (**google/gemini-2.5-flash-lite**) to convert to markdown, then creates a folder under `meeting-notes/` named from the related issue’s title and writes `summary.md` and `transcript.md` there. Commits and pushes, then comments on the issue with links.

**Inputs:** (when you run it manually)
- **google_doc_url** — Public Google Doc URL. Doc must be shared as **Anyone with the link can view**.
- **issue_number** — The meeting issue number (e.g. `42`). The issue title is used for the folder name (e.g. `Weekly sync — 2026-02-10` → `meeting-notes/weekly-sync-2026-02-10/`).

**Setup:**
- **OPENROUTER_API_KEY** — In the repo on GitHub: **Settings → Secrets and variables → Actions → New repository secret**. Name: `OPENROUTER_API_KEY`, value: your [OpenRouter](https://openrouter.ai) API key.

**How to run:** **Actions → Google Doc → Meeting notes → Run workflow**, then fill in the doc URL and issue number.
