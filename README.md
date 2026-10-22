# salucallc/.github

Organization-wide community health defaults for [salucallc](https://github.com/salucallc) repositories.

GitHub automatically applies the contents of this repository as default templates for any salucallc repo that does not override them locally. Repo-local files always win.

## Status

Maintained. Today it provides the files listed under Usage. It covers the `salucallc` organization only: GitHub applies an org's `.github` repo to that org's repos, so `saluca-labs` repos do not inherit these files.

### Corrections, 2026-10-22

This README described several things this repo does not contain or do:

- It listed issue templates for "bug report, feature request, security (pointer), config gating contact links". Only the bug report and feature request templates exist; there is no security template and no `config.yml`.
- It said `CODE_OF_CONDUCT.md` is the Contributor Covenant 2.1. It is a shorter code of conduct written for Saluca, not the Contributor Covenant.
- It listed a `CODEOWNERS` file with a default owner. There is no `CODEOWNERS` file here, and GitHub does not apply `CODEOWNERS` from an org's `.github` repo to other repos.
- It listed default workflows in `.github/workflows/`. There is no workflows directory. GitHub does not run workflows from this repo in other repos; reusable workflows live in [`salucallc/ci-shared`](https://github.com/salucallc/ci-shared).
- Under Maintenance it said direct pushes to `main` are disabled and that Dependabot bumps action pins weekly. On 2026-10-22 `main` had no branch protection or ruleset, and there is no Dependabot configuration in this repo (it has no workflows to bump).

## Install

Nothing to install. GitHub reads these files from this repository; consuming repos do nothing.

## Quickstart

Open the security policy of a salucallc repo that has no `SECURITY.md` of its own, for example
<https://github.com/salucallc/ci-shared/security/policy>. GitHub shows this repo's [SECURITY.md](SECURITY.md)
there, with the `security@saluca.com` reporting address.

## Usage

What this repo provides:

| File | Used by GitHub as |
|---|---|
| [`SECURITY.md`](SECURITY.md) | the security policy (reporting address `security@saluca.com`) |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | the contributing guidelines |
| [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) | the code of conduct (reports to `conduct@saluca.com`) |
| [`.github/ISSUE_TEMPLATE/bug_report.md`](.github/ISSUE_TEMPLATE/bug_report.md) | the "Bug report" issue template |
| [`.github/ISSUE_TEMPLATE/feature_request.md`](.github/ISSUE_TEMPLATE/feature_request.md) | the "Feature request" issue template |
| [`.github/pull_request_template.md`](.github/pull_request_template.md) | the pull request template |
| [`profile/README.md`](profile/README.md) | the text on the [salucallc organization page](https://github.com/salucallc) |

A repo overrides any of these by adding its own file of the same name. For CI, a repo adds a thin workflow at `.github/workflows/ci.yml` that calls the reusable workflows in [`salucallc/ci-shared`](https://github.com/salucallc/ci-shared); see its README for the call surface and pinning guidance.

## Architecture

There is no code. GitHub looks for each community health file in the repo itself first, then in this repo (at the root or in `.github/`). This repo must stay public for that to work. `LICENSE` and `README.md` here describe this repo only and are not inherited.

## Maintenance

- Changes land via PR to `main`.
- A change here changes every salucallc repo that does not override the file, so keep the files general and free of internal details.

## Citation

No archived record yet.

## License

MIT. See [LICENSE](LICENSE). Templates are intentionally liberal so forks and external contributors can reuse them.

## Links

- [salucallc/ci-shared](https://github.com/salucallc/ci-shared): reusable GitHub Actions workflows
- [GitHub docs: default community health files](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)

_Last updated: 2026-10-22_
