# AGENTS.md

Instructions for AI coding agents, and a short version for anyone working here.

## What this repository is

`.github` holds the shared defaults for every public repository in the USAREUR-AF organization. GitHub uses the issue templates and the pull request template here for any repository that does not have its own. The workflows here are the organization's shared checks, `verified-commits` and `contributor-trust`.

## Layout

| Path | What |
|---|---|
| `.github/ISSUE_TEMPLATE/` | bug report, feature request, and the links for security reports and questions |
| `.github/PULL_REQUEST_TEMPLATE.md` | the pull request checklist |
| `.github/workflows/` | `verified-commits.yml` and `contributor-trust.yml` |
| `.github/contributor-trust/` | the list of sensitive paths that `contributor-trust` reads |

## Before you push

There is nothing to build. A change here reaches every repository that has no copy of its own, so keep each file short and general, and read the changed template or workflow once more as it will appear in another repository.

## Rules

1. **Commits.** Conventional Commits subject of 100 characters or fewer, with a scope (`fix(<component>): …`). Every commit is signed off (`git commit -s`, the DCO) and signed with a key GitHub verifies. The required check `verified-commits` refuses a pull request that holds an unverified commit.
2. **One logical change per pull request.**
3. **Nothing that belongs to one repository or one deployment.** A repository that needs something different keeps its own copy, and that copy wins.

The contribution guide for goat as a whole is [goatcore CONTRIBUTING.md](https://github.com/USAREUR-AF/goatcore/blob/main/CONTRIBUTING.md).
