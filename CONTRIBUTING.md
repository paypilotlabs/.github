# Contributing to PayPilotLabs

Thanks for helping. This guide applies to every PayPilotLabs repo unless the repo has its own.

## Find an issue

1. Pick an issue labelled `good first issue`.
2. Comment on it to ask for it.
3. Wait to be assigned before you start.

One person works on each issue. If an assigned issue has no update for 10 days, it gets unassigned.

## Workflow

1. Fork the repo. Outside contributors do not get write access.
2. Create a branch from `main`. Use a prefix: `feat/`, `fix/` or `docs/`. Example: `fix/login-timeout`.
3. Write commit messages in [Conventional Commits](https://www.conventionalcommits.org/) format. Example: `fix: stop login timing out after 30s`.
4. Open one pull request per issue.
5. Put `Closes #N` in the pull request body, where `N` is the issue number.

## Before you open a pull request

- Tests and lint pass on your machine.
- New behaviour has tests.
- Docs are updated if behaviour changed.

## CI

For first-time contributors, CI runs only after a maintainer approves it. This is normal. You do not need to do anything.

## Secrets and personal data

Never commit secrets, `.env` files, API keys or personal data. If you commit one by mistake, tell us in the pull request. Deleting it in a later commit is not enough.

## Licence

Your contribution is licensed under the repo's own licence (inbound = outbound). Check the `LICENSE` file in the repo you are contributing to.

## Review

- @squid-beast reviews and merges pull requests. Merges are squashed.
- Reply to review comments and push your changes to the same branch.
- Pull requests with no activity for 14 days are closed. You can reopen when you are ready.

## Recognition

Merged contributors are credited in the release notes and the README. PayPilotLabs also gives you a shout-out on LinkedIn and X. Tag @paypilotlabs when you share your work.

## Security problems

Do not open a public issue for a security problem. Follow [SECURITY.md](SECURITY.md).

## Code of conduct

Everyone taking part follows our [Code of Conduct](CODE_OF_CONDUCT.md).
