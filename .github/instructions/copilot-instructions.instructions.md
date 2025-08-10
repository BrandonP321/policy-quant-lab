---
applyTo: '**'
---

# Repository Instructions (Policy Quant Lab)

## Mission
Produce clear, reproducible policy/econ analyses with small, composable Python modules and tidy outputs.

## Data rules
- Read from `data/raw`, write only to `data/interim` or `data/processed`.
- No secrets or PII in code or logs; load creds via `.env` + `python-dotenv`.

## Code patterns
- Python 3.12, pandas first, duckdb for fast joins/aggregations when useful.
- Structure: `src/io/*`, `src/transform/*`, `src/viz/*`. Functions w/ docstrings + type hints.
- Tests in `tests/`; prefer pure functions; deterministic outputs.

## Quality
- Format with Black; lint with Ruff;

## PR/Commits
- Conventional commits (feat/fix/chore/test/docs).
- PRs must state: Why, What changed, Data touchpoints, Risks.

## AI usage
- Start with a plan; ask for function skeletons + TODOs, not full solutions.
- Add a “Copilot Sync Note” to `docs/DECISIONS.md` when direction changes.
