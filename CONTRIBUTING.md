# Contributing to Stock Analyzer

First off — thank you for your interest in contributing to Stock Analyzer! Your contributions (code, documentation, tests, bug reports, or ideas) help make this project better for everyone.

This document explains how to report bugs, propose features, and submit changes so your contribution can be reviewed and merged quickly.

---

## Table of contents

- [Code of Conduct](#code-of-conduct)
- [How to get help / ask questions](#how-to-get-help--ask-questions)
- [Reporting bugs](#reporting-bugs)
- [Suggesting improvements / feature requests](#suggesting-improvements--feature-requests)
- [Before you start coding](#before-you-start-coding)
  - [Set up a development environment](#set-up-a-development-environment)
  - [Style & linters](#style--linters)
  - [Branching and commit messages](#branching-and-commit-messages)
- [How to submit a pull request (PR)](#how-to-submit-a-pull-request-pr)
- [Testing](#testing)
- [Data & privacy considerations](#data--privacy-considerations)
- [Security issues](#security-issues)
- [Maintainers & response time](#maintainers--response-time)
- [Thanks!](#thanks)

---

## Code of Conduct

We expect everyone participating in this project to follow a respectful, inclusive Code of Conduct. By participating, you agree to abide by it. If we don't already have a separate `CODE_OF_CONDUCT.md` file in the repo, please follow these basics:
- Be respectful and patient.
- Report harassment or abusive behavior privately to the maintainers.

(If you'd like, we can add a full Contributor Covenant or a project-specific code of conduct.)

---

## How to get help / ask questions

- Search existing issues first to see if your question has been asked.
- For quick questions, open a new issue with the label `question` and include:
  - A clear subject line
  - Repro steps or a short code snippet
  - Environment (OS, Python/Node/other version, Stock Analyzer version)

---

## Reporting bugs

When filing a bug report, please include as much of the following as possible:

- A descriptive title and a short summary.
- Steps to reproduce the bug (minimal reproducible example if possible).
- What you expected to happen and what actually happened.
- Logs, stack traces, or screenshots (if applicable).
- Environment information:
  - OS and version
  - Stock Analyzer version (commit/branch/tag)
  - Language/runtime versions (e.g., Python 3.11, Node 18)
  - Any relevant configuration (API keys removed)
- If the bug is related to a dataset, include a small sample (dummy or synthetic) that reproduces the issue, not real/private data.

Label your issue as `bug` and add the appropriate severity (e.g., `critical`, `major`, `minor`) if you can.

---

## Suggesting improvements / feature requests

To propose a feature:
- Open an issue titled “Feature: Short description”.
- Explain:
  - The problem you’re trying to solve.
  - Why it matters and who benefits.
  - A concrete proposal for how it might work (API, UI, CLI).
  - Alternatives you considered.
  - Any backward-compatibility concerns.

If your feature is large, consider opening an RFC or design issue first so maintainers can provide early feedback.

---

## Before you start coding

1. Check open issues for related work — you may want to comment that you're working on it.
2. If your change is large or architectural, open a short design discussion issue first.

### Set up a development environment

Below are example steps. Adjust to match the repo's language/tooling.

For a Python-based setup:
```bash
git clone https://github.com/<owner>/stock-analyzer.git
cd stock-analyzer
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

For a Node/TypeScript setup:
```bash
git clone https://github.com/<owner>/stock-analyzer.git
cd stock-analyzer
npm install
```

(Replace `<owner>` with the repository owner.)

### Style & linters

- Follow the repository's existing formatting and style. If the repo uses:
  - Python: use `black` and `flake8` or `ruff`.
  - JS/TS: use `prettier` and `eslint`.
- Run linters and formatters before opening a PR.

### Branching and commit messages

- Fork the repo (unless you have push access), then create a branch from `main`:
  - `feature/<short-description>` for new features
  - `fix/<issue-number>-short-description` for fixes
  - `chore/<short>` for maintenance
- Follow Conventional Commits for commit messages:
  - Format: `type(scope?): subject`
  - Examples:
    - `feat(indicators): add MACD crossover detector`
    - `fix(data): handle missing timestamps in CSV import`
    - `docs: update contributing guide`

Squash/fixup commits as appropriate before merge (maintainers may rebase).

---

## How to submit a pull request (PR)

1. Fork and create a branch as described above.
2. Make small, focused changes per PR.
3. Add or update tests for new behavior.
4. Update documentation where applicable.
5. Push your branch to your fork and open a PR against `main` (or the branch specified by maintainers).
6. In your PR description, include:
   - A short summary of changes.
   - Issue number (if applicable): `Closes #123`
   - Steps to test / reproduction steps.
   - Any migration steps or breaking changes.

PR checklist (please tick before requesting review):
- [ ] My code follows the repository style conventions
- [ ] I added tests that prove my fix/feature works
- [ ] I updated documentation (README, docs/) where applicable
- [ ] All CI checks pass locally and on the PR
- [ ] I linked the related issue(s)

---

## Testing

- Run the test suite before opening a PR:
  - Python example: `pytest`
  - Node example: `npm test`
- Aim for high coverage for new features. If a change is complex, include unit and integration tests.
- If your change requires new test data, prefer synthetic or very small extracts, and do not commit proprietary data.

---

## Data & privacy considerations

Stock Analyzer may process financial data. When contributing:
- Do NOT commit API keys, credentials, or sensitive/private data.
- Use environment variables or config files that are ignored by `.gitignore`.
- If you add example datasets, ensure they are synthetic or anonymized and have appropriate licensing.
- Document expected data schema and formats for any new data sources or ingesters.

---

## Security issues

If you discover a security vulnerability, do NOT open a public issue. Contact the maintainers privately. You can:
- Email: (add a maintainer email here)
- Or open a GitHub Security Advisory if enabled.

Please include steps to reproduce and potential impact.

---

## Maintainers & response time

Primary maintainers:
- @ruthviksharma-d

We aim to respond to new issues and PRs within 3–7 business days. Larger changes may take longer due to review and testing.

---

## Licensing and contributor agreement

By submitting a PR, you agree that your contributions will be licensed under the project's license (see `LICENSE`). If your employer requires a Contributor License Agreement (CLA), maintainers will provide one if needed.

---

## Large contributions & roadmap-aligned work

If you plan to implement a major feature (architecture changes, new analysis engine, large refactor), please:
1. Open a design/roadmap issue describing the approach.
2. Tag it `design` or `proposal`.
3. Wait for maintainer feedback before investing significant time.

---

## Thank you

Thanks again for contributing! Your help improves the project for everyone. If you'd like help getting started, consider looking for issues labeled `good first issue` or `help wanted`.

If you'd like, I can also:
- create a ready-to-use PR template and issue templates for this repository,
- or adapt this CONTRIBUTING.md with language-specific setup commands (Python, Node, etc.). Let me know which stack your project uses.
