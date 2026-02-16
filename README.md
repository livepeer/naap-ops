# naap-ops

Central place for Network-as-a-Product operations. This repo holds decisions, docs, and meeting notes so the team and AI agents have a single source of truth. Workflows capture meeting notes and notify contributors (e.g. weekly sync issues). See the sections below for structure, meetings, and workflows.

---

## Structure

| Path | Purpose |
|------|---------|
| [decisions/](decisions/) | ADRs and key decisions |
| [docs/](docs/) | General project docs, onboarding, references |
| [meeting-notes/](meeting-notes/) | Notes, outcomes |

## Meetings

| Meeting | Agenda | Notes |
|---------|--------|--------|
| **Weekly sync** | Agenda created automatically as a GitHub issue (Mondays 9:00 UTC). Contributors are tagged to post progress and questions. No Agenda = No Air Time | Add notes in [meeting-notes/](meeting-notes/); link from the issue. Weekly sync is scheduled for Tuesdays at 5pm GMT. Join [here](https://meet.google.com/qjy-fxrn-sft?authuser=0&hs=122&ijlm=1770912842702)  |
| **Other meetings** | Open a GitHub issue for the meeting. | Add the meeting note in `meeting-notes/`, then close the issue (e.g. with a comment linking to the note). Any decisions from the meeting go in [decisions/](decisions/). |

## Workflows
Access workflows in Github Actions.
| Workflow | What it does |
|----------|--------------|
| **Weekly meeting issue** | Mondays 9:00 UTC: creates a meeting issue and a comment that tags contributors to post progress and questions (no questions = no air time). |
| **Weekly sync agenda** | Mondays 16:00 UTC: finds that week’s weekly sync issue, reads all comments, and updates the issue body with agenda items from those comments. |
| **Google Doc → Meeting notes** | Manual run: give a public Google Doc URL and issue number → creates a PR that adds `meeting-notes/{issue-title}/summary.md` and `transcript.md` (Closes the issue when merged). |

Details and setup (e.g. secrets): [docs/workflows.md](docs/workflows.md).

## Usage

- **Single source of truth**: Cross-repo context lives here; code stays in respective repos.
- **Decisions**: One file per decision in `decisions/`.
- **AI-friendly**: Flat structure and markdown so agents can read and reason over the same info as humans.