# naap-ops

Project management and operations for the NAAP initiative across repos and orgs.

## Structure

| Path | Purpose |
|------|---------|
| [decisions/](decisions/) | ADRs and key decisions |
| [docs/](docs/) | General project docs, onboarding, references |
| [meeting-notes/](meeting-notes/) | Notes, outcomes |

## Meetings

| Meeting | Agenda | Notes |
|---------|--------|--------|
| **Weekly sync** | Agenda created automatically as a GitHub issue (Mondays 9:00 UTC). Contributors are tagged to post progress and questions. No Agenda = No Air Time | Add notes in [meeting-notes/](meeting-notes/); link from the issue.  |
| **Other meetings** | Open a GitHub issue for the meeting. | Add the meeting note in `meeting-notes/`, then close the issue (e.g. with a comment linking to the note). Any decisions from the meeting go in [decisions/](decisions/). |

## Workflows
Access workflows in Github Actions.
| Workflow | What it does |
|----------|--------------|
| **Weekly meeting issue** | Mondays 9:00 UTC: creates a meeting issue and a comment that tags contributors to post progress and questions (no questions = no air time). |
| **Google Doc → Meeting notes** | Manual run: give a public Google Doc URL and issue number → creates a PR that adds `meeting-notes/{issue-title}/summary.md` and `transcript.md` (Closes the issue when merged). |

Details and setup (e.g. secrets): [docs/workflows.md](docs/workflows.md).

## Usage

- **Single source of truth**: Cross-repo context lives here; code stays in respective repos.
- **Decisions**: One file per decision in `decisions/`.