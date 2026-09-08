# Project state

**Last updated:** 2026-09-08  
**Current milestone:** Milestone 0 — design lock and collaboration setup  
**Repository:** [rishic999/momentum-continuation-research](https://github.com/rishic999/momentum-continuation-research)  
**Default branch:** `main`

## Current objective

Establish the durable operating system for a reproducible study of momentum continuation after a large stock run-up. The research question and first-pass methodology are documented; implementation has not begun.

## Completed

- Defined the primary competing-risk question: after a qualifying large run, does a stock reach +20% before -10% within 60 trading days?
- Wrote the research charter, literature map, methodology, data plan, and staged roadmap.
- Created and published the public GitHub repository.
- Added the agent operating contract and this project-state handoff.

## Key current decisions

- The project estimates calibrated conditional probabilities, not individual-stock certainty or investment recommendations.
- A point-in-time, event-level panel is required; later-revised information must not enter historical decision rows.
- Price-only baselines come before earnings/revision data, NLP, options data, or machine learning.
- `main` remains reproducible; use branches/worktrees for parallel work.

## Known blockers / open choices

- Select the initial historical price-data source and document its survivorship, adjustment, delisting, and licensing limitations.
- Set the pre-registered study period and exact liquidity floor once data availability is known.
- Decide whether Milestone 1 should prioritize a fully reproducible public-data prototype or a higher-quality licensed-data pipeline.

## Best next task

Create a short data-source decision memo comparing feasible point-in-time U.S. equity price datasets for Milestone 1. It must recommend one source, state known biases/limitations, and map the source fields to the price-only event-panel requirements.

## Validation status

- Documentation links and whitespace check: pending after this change.
- No research code or data pipeline exists yet.

