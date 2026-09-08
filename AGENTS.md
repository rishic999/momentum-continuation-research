# Momentum Continuation Research — agent operating contract

This repository is a durable, public research record. Every agent must preserve its reproducibility, clarity, and honest distinction between a hypothesis, an exploratory result, and a validated finding.

## Required start-of-task protocol

Before taking substantive action, read:

1. `README.md`
2. `docs/research-charter.md`
3. `docs/project-state.md`
4. `docs/decisions.md`
5. the files directly relevant to the assigned task

Then inspect `git status` and recent commits. If the task conflicts with the charter or a recorded decision, flag the conflict rather than silently changing scope.

## Required completion protocol

Before declaring a task complete, every agent must:

1. Update `docs/project-state.md` with completed work, current findings, blockers, and the single best next task.
2. Add a dated entry to `docs/decisions.md` for any durable choice, changed assumption, rejected approach, or material interpretation.
3. Update the relevant public documentation whenever code, data definitions, methodology, or results change.
4. Run proportionate validation and record the exact command/result in `docs/project-state.md`.
5. Commit the coherent change with a descriptive message and push it when remote access is available.

Do not leave required handoff information only in a chat transcript. A future chat must be able to orient itself from the repository alone.

## Research integrity requirements

- Use only information available at each decision timestamp; document all availability assumptions.
- Do not overwrite raw data or commit licensed, private, credentialed, or redistributable-restricted data.
- Treat a result as exploratory unless it survives the pre-specified temporal validation plan.
- Never tune thresholds, features, horizons, or universes on the final test period.
- Preserve negative results and failed experiments in the decision log or an exploratory report.
- Do not turn results into investment recommendations.

## Repository conventions

- `docs/`: durable design, data, state, decisions, and findings.
- `src/`: reusable production research code, not one-off exploration.
- `notebooks/`: exploration; promote stable logic into `src/` and tests.
- `tests/`: automated checks for labels, timestamps, transformations, and data quality.
- `reports/`: reproducible research outputs, never undocumented manual conclusions.
- `data/`: ignored local data only; commit schemas, acquisition instructions, and synthetic fixtures instead.

## Parallel work

Use separate branches/worktrees for concurrent tasks. Do not modify another task’s in-progress changes. Keep `main` reproducible; merge only complete, documented work.

