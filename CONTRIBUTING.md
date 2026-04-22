# Contributing to Saluca LLC projects

Most Saluca products are dual-licensed: a Noncommercial / research tier under PolyForm Noncommercial 1.0.0, and a commercial SKU. Contributions to any Saluca repo are accepted under the same licensing terms as the repo itself.

## Before you open a PR

1. Check the repo's `README.md` for project-specific contribution notes.
2. Open an issue first for anything larger than a bug fix or a typo — a short design alignment is cheaper than a big PR that gets redirected.
3. Sign commits if the repo requires it (most product repos do; see the repo settings).

## Scope discipline

- One change per PR. Separate refactors, fixes, and features.
- No backwards-compatibility shims unless specifically asked.
- No speculative abstractions. Three similar lines beats a premature framework.
- Add tests for behavior changes.

## Style

- Match the surrounding code. Run any linter or formatter the repo ships.
- Commit messages concrete: what changed and why.

## License + CLA

By submitting a contribution, you agree that the work may be licensed under the repo's declared license, and that you have the rights to license it that way. No separate CLA is required for most repos; some product repos may require one and will surface that on the PR.

## Security

See `SECURITY.md`. Do not open public issues for security findings.
