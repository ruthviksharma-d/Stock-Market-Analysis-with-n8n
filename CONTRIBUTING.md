# Contributing to My-own-photoshop-webapp-in-7-days

Thank you for your interest in contributing! We welcome contributions of all kinds — bug reports, feature requests, documentation improvements, tests, and code. This document explains how to get started and the process we use to review and accept contributions.

## Table of Contents
- How can I contribute?
- Getting started (fork & clone)
- Development setup
- Coding conventions
- Branching & Pull Requests
- Commit messages
- Running tests & linting
- Submitting issues
- Pull request checklist
- Code of Conduct
- License

## How can I contribute?
- Report bugs or request features by opening an issue.
- Submit a fix or new feature via a pull request.
- Improve documentation, examples, or the README.
- Help with triage: label issues, reproduce bugs, answer questions.

## Getting started
1. Fork the repository on GitHub.
2. Clone your fork:
   - SSH: `git clone git@github.com:<your-username>/My-own-photoshop-webapp-in-7-days.git`
   - HTTPS: `git clone https://github.com/<your-username>/My-own-photoshop-webapp-in-7-days.git`
3. Add the upstream remote:
   - `git remote add upstream https://github.com/ruthviksharma-d/My-own-photoshop-webapp-in-7-days.git`
4. Create a branch for your work:
   - `git checkout -b feat/short-description` or `git checkout -b fix/short-description`

## Development setup
This project is a web application. Typical steps (adjust to actual project tooling):

- Install dependencies:
  - `npm install` or `yarn install`
- Start the dev server:
  - `npm run dev` or `yarn dev`
- Build for production:
  - `npm run build` or `yarn build`
- Run tests:
  - `npm test` or `yarn test`

If the project uses different commands or additional services (e.g., Docker), check the README for specific instructions. If no README instructions exist, open an issue or start a discussion so we can document the setup.

## Coding conventions
- Keep code readable and well-documented.
- Follow the existing style. If you add new tooling (ESLint, Prettier), include config files and document how to run them.
- Prefer small, focused commits that are easy to review.
- Add or update tests for new functionality or bug fixes.
- Write clear commit messages (see below).

Recommended:
- Use eslint + prettier (or the project's chosen linter/formatter).
- Prefer modern JavaScript/TypeScript patterns consistent with the repository.

## Branching & Pull Requests
- Fork the repo and work in a branch named with the pattern `feat/` or `fix/` followed by a short description, e.g. `feat/image-crop`.
- Rebase or pull the latest changes from `upstream/main` (or main branch) before opening a PR.
- Push your branch to your fork and open a Pull Request against `ruthviksharma-d:main`.
- In your PR description, describe:
  - What you changed and why
  - Any related issues (e.g., `Closes #123`)
  - How to test or reproduce
  - Screenshots if the change affects UI

PRs will be reviewed by repository maintainers. Be responsive to review feedback and update your PR as requested.

## Commit messages
Use clear, imperative-style messages. Optionally follow Conventional Commits:

- feat: add a new feature
- fix: fix a bug
- docs: documentation only changes
- style: formatting, missing semi-colons, etc.
- refactor: code changes that neither fixes a bug nor adds a feature
- test: adding missing tests or correcting existing tests
- chore: changes to the build process or auxiliary tools

Example:
```
feat: add image-export feature (png, jpeg)

- add export dialog
- support quality slider
- update README with usage
```

## Running tests & linting
- Run the test suite locally before opening a PR: `npm test`
- Run linter/formatter: `npm run lint` and `npm run format` (or project-specific commands)
- Make sure all tests pass and lint errors are resolved

## Submitting issues
- Search issues to avoid duplicates.
- Use a clear title and include steps to reproduce, expected vs actual behavior, environment (OS, browser, node version), and screenshots or logs if helpful.
- Tag issues as `bug`, `enhancement`, `question`, etc., and include `good first issue` if you think it’s suitable for newcomers.

## Pull request checklist
Before requesting a review, please make sure:
- [ ] You have read the Code of Conduct.
- [ ] Your PR is against the `main` branch.
- [ ] The changes are limited to a single purpose.
- [ ] Tests are added/updated where applicable.
- [ ] Linting and formatting pass.
- [ ] Documentation/README updated if necessary.
- [ ] All CI checks (if any) are passing.

## Documentation & Examples
If you add or change functionality, update the README or relevant docs with usage examples, configuration options, and any new commands or environment variables.

## Questions or help
If you're unsure where to start, check for issues labelled `help wanted` or `good first issue`. You can also open an issue to ask for guidance.

## Code of Conduct
This project follows the Contributor Covenant Code of Conduct. By participating, you agree to abide by its terms: see CODE_OF_CONDUCT.md.

## License
Contributions to this repository are subject to the repository's license. Please review the LICENSE file in the repository before contributing.

---

Thanks again for helping improve this project — contributions keep open source projects alive and growing. If you have suggestions for improving this contribution guide, please open a pull request or an issue.
