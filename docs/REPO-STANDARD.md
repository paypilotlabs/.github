# Repo standard

Every PayPilotLabs repo must pass this checklist before it goes public.

## Access

- [ ] No outside collaborator has write access.
- [ ] Outside contributors work through fork + pull request only.
- [ ] The org requires two-factor authentication.

## Ruleset: "main protection"

Settings > Rules > Rulesets. Target the default branch.

- [ ] Restrict deletions.
- [ ] Block force pushes.
- [ ] Require a pull request before merging, with 1 approval.
- [ ] Dismiss stale approvals when new commits are pushed.
- [ ] Require review from Code Owners.
- [ ] Require conversation resolution before merging.
- [ ] Require status checks to pass (add the CI job).
- [ ] Bypass list: Repository admin, set to pull requests only.

## Actions

Settings > Actions > General.

- [ ] Require approval for all external contributors.
- [ ] Workflow permissions: read repository contents only.
- [ ] Actions cannot create or approve pull requests.
- [ ] No workflow uses `pull_request_target` with code from a fork.
- [ ] Third-party actions are pinned to full commit SHAs, with the version in a comment.

## Advanced Security

Settings > Advanced Security.

- [ ] Dependency graph on.
- [ ] Dependabot alerts on.
- [ ] Dependabot security updates on.
- [ ] Secret scanning on, with push protection.
- [ ] Private vulnerability reporting on.
- [ ] CodeQL default setup on.

## Files

These must be in the repo itself:

- [ ] `LICENSE`
- [ ] `README.md`
- [ ] `.github/CODEOWNERS` (copy from `templates/CODEOWNERS`)
- [ ] `.github/dependabot.yml` (copy from `templates/dependabot.yml`)
- [ ] A CI workflow in `.github/workflows/` (start from `workflow-templates/ci-node.yml`)

Community files (`CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, `SUPPORT.md`, issue and pull request templates) come from the `paypilotlabs/.github` repo unless the repo has its own.

## Secrets

- [ ] Secrets live only in GitHub secret settings or Vercel environment settings.
- [ ] No secret is ever committed to git.
