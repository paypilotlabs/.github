# .github

Org-wide defaults for PayPilotLabs. GitHub applies the community files in this repo to every public `paypilotlabs` repo that does not have its own copy.

## Files GitHub inherits

| File | What it does |
| --- | --- |
| `CONTRIBUTING.md` | How to pick an issue, open a pull request, and get it merged. |
| `CODE_OF_CONDUCT.md` | Contributor Covenant v2.1. |
| `SECURITY.md` | How to report a vulnerability privately. |
| `SUPPORT.md` | Where to ask questions and where to send business enquiries. |
| `FUNDING.yml` | Adds the Sponsor button that links to GitHub Sponsors. |
| `.github/ISSUE_TEMPLATE/` | Bug report and feature request forms. Blank issues are off. Security reports are sent to private reporting. |
| `.github/pull_request_template.md` | The default pull request body and checklist. |

A repo that has its own version of a file uses that file instead. A repo with any file in its own `.github/ISSUE_TEMPLATE/` folder gets none of the issue templates from here.

## Other files

| File | What it does |
| --- | --- |
| `profile/README.md` | The public page at github.com/paypilotlabs. |
| `workflow-templates/ci-node.yml` | Starter CI for Node repos. It shows up under Actions > New workflow. It is offered, not applied. |
| `templates/CODEOWNERS` | Code owners file. |
| `templates/dependabot.yml` | Weekly Dependabot updates for npm and GitHub Actions. |
| `docs/REPO-STANDARD.md` | The checklist every repo must pass before it goes public. |

## Not inherited

GitHub does not apply these to other repos. Copy them in by hand:

- `templates/CODEOWNERS` goes to `.github/CODEOWNERS`.
- `templates/dependabot.yml` goes to `.github/dependabot.yml`.
- `workflow-templates/ci-node.yml` goes to `.github/workflows/ci.yml` (or add it from the Actions tab).
