# Momentum Continuation Research

An empirical, reproducible study of a narrow question: after a stock has already made a large, fundamentals-supported move, when is continuation more likely than failure?

This is a research project, not investment advice or a live trading system. Its purpose is to test ideas honestly using point-in-time data, transparent definitions, and out-of-sample evaluation.

## Research question

For a liquid U.S. equity that has already experienced a large upward move, can information available on the decision date—earnings surprise and guidance, estimate revisions, price/volume trend quality, peer confirmation, and risk regime—improve the estimate that it will reach a further upside target before a defined drawdown?

The exact first-pass specification, hypotheses, scope, and failure criteria live in [docs/research-charter.md](docs/research-charter.md).

## What this is and is not

- **Is:** a cross-sectional, event-conditioned study of continuation after large runs.
- **Is:** a framework for probabilities and payoff distributions, not certainty.
- **Is not:** an attempt to forecast NVDA or any one stock in isolation.
- **Is not:** a recommendation to buy securities or options.

## Repository map

- [Research charter](docs/research-charter.md) — the decision document and scope guardrails.
- [Literature map](docs/literature-map.md) — what established research answers and the remaining gap.
- [Methodology](docs/methodology.md) — event definition, labels, features, validation, and metrics.
- [Data plan](docs/data-plan.md) — required datasets, point-in-time rules, and phased sourcing.
- [Project roadmap](docs/roadmap.md) — staged deliverables and explicit go/no-go gates.

## Initial workflow

1. Assemble an immutable point-in-time event panel for liquid U.S. equities.
2. Run transparent baselines before adding complex features.
3. Evaluate forward outcomes with a purged, chronological test design.
4. Compare every model with simple benchmarks and report uncertainty.
5. Publish negative as well as positive results.

## Status

The repository currently contains the research design and implementation plan. The first coding milestone is the price-only event panel and baseline continuation analysis.

