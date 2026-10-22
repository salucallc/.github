# AGENTS.md

Instructions for AI coding agents working in this repository.

## Setup

Nothing to install. The repo is Markdown files that GitHub reads as defaults for every salucallc repo.

## Test

There is no test suite. Before a PR, check that every link in README.md and llms.txt resolves and that
`llms-full.txt` matches the docs.

## Conventions

- Every file here is shown in every salucallc repo that lacks its own copy. Keep the text general:
  no repo-specific instructions, internal tool names, hostnames, internal paths or personal addresses.
- Contact addresses are role addresses (`security@saluca.com`, `conduct@saluca.com`).
- When any doc changes, regenerate `llms-full.txt` in the same PR: the `llms.txt` header, then each file
  under a `## <path>` heading in the order README.md, SECURITY.md, CONTRIBUTING.md, CODE_OF_CONDUCT.md,
  .github/ISSUE_TEMPLATE/bug_report.md, .github/ISSUE_TEMPLATE/feature_request.md,
  .github/pull_request_template.md, profile/README.md.
- No em-dashes.

## Do not

- Describe files that do not exist here (CODEOWNERS and workflows are not inherited from this repo).
- Make this repo private: GitHub only applies defaults from a public `.github` repo.
- Commit secrets, hostnames, internal paths or personal emails.

## Done means

Links resolve, README.md describes exactly the files present, and `llms-full.txt` is regenerated.
