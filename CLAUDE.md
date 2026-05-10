# CLAUDE.md

## Repository Purpose

Personal dotfiles and daily-work scripts for managing configurations across various environments (Linux, Windows).

## Known Structure

- `experiments/` — deliberate playground and backup directory, not production code; ignore when reviewing
  - `experiments/superpowers/` — brainstorming specs and implementation plans from Claude sessions (gitignored, local only); check here for prior design decisions before starting new work
- `node_modules/` — exists locally but is gitignored; not committed to the repo

## Tooling

- Renovate: `renovate.json` in `.github/` is the repository-specific Renovate entry point; the `schedule` override there is intentional
- pre-commit hook runs `lint-staged` (Prettier + cspell) on `*.json`, `*.md`, `*.yml`; additionally runs `js-yaml` syntax validation on `*.yml`, `*.yaml`
