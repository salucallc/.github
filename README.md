# salucallc/.github

Organization-wide community health defaults for [salucallc](https://github.com/salucallc) repositories.

GitHub automatically applies the contents of this repository as default templates for any salucallc repo that does not override them locally. Repo-local files always win.

## What this repo provides

- **Issue templates** (`.github/ISSUE_TEMPLATE/`) — bug report, feature request, security (pointer), config gating contact links.
- **PR template** (`.github/pull_request_template.md`) — derived from the gmail-mcp template; lightweight, privacy/compliance-aware.
- **SECURITY.md** — canonical vulnerability-reporting policy pointing to `security@saluca.com`.
- **CODE_OF_CONDUCT.md** — Contributor Covenant 2.1.
- **CODEOWNERS** — default owner `@cristianxruvalcaba-coder`; repos SHOULD override with a local CODEOWNERS when they have specific subtree reviewers.
- **Default workflows** (`.github/workflows/`) — opt-in, one-line `uses:` references to reusable workflows in [`salucallc/ci-shared`](https://github.com/salucallc/ci-shared).

## How repos consume this

For community health files (issue templates, PR template, SECURITY, COC): no action required. GitHub surfaces them automatically unless the repo defines its own.

For CI: add a thin workflow at `.github/workflows/ci.yml` in the consuming repo that calls the reusable workflows from `ci-shared`. See `salucallc/ci-shared` README for the current call surface and pinning guidance.

## Licensing

MIT. See `LICENSE`. Templates are intentionally liberal so forks and external contributors can reuse them.

## Maintenance

- All changes land via PR to `main`; direct pushes to `main` are disabled.
- Third-party actions in any default workflow MUST be SHA-pinned; Dependabot is configured to bump pins weekly.
- When the upstream `salucallc/gmail-mcp` CI template evolves, promote stable changes into the reusable workflows in `ci-shared` and update the default workflows here to reflect the new call surface.
