# Roadmap and decision gates

## Milestone 0 — design lock

Deliverables: research charter, literature map, data plan, repository conventions.

Gate: no implementation parameter is changed without documenting whether it is pre-registered or exploratory.

## Milestone 1 — price-only event panel

Deliverables: point-in-time universe, event detector, barrier labels, descriptive event study, and data-quality tests.

Gate: verify dates, splits/dividends, delistings, overlapping-event treatment, and label logic on hand-checked examples.

## Milestone 2 — transparent baselines

Deliverables: unconditional, price-only, and regime-aware results with walk-forward validation.

Gate: stop if baseline effects are not stable or cannot survive conservative implementation assumptions.

## Milestone 3 — earnings and revisions

Deliverables: earnings-event features, estimate-revision features, incremental-value analysis against Milestone 2.

Gate: retain only features that improve final-period calibration and economic outcomes.

## Milestone 4 — peers and risk overlays

Deliverables: industry/thematic confirmation and market-regime risk analysis.

Gate: distinguish a better return forecast from merely taking more risk.

## Milestone 5 — exploratory additions

Deliverables: options and transcript-NLP experiments, isolated in an exploratory appendix.

Gate: nothing moves into the core model without reproducible point-in-time data and a separate final test.

## Publication standard

Publish a reproducible report, all definitions, tests, data-access limitations, and negative results. State clearly that results are historical and not investment advice.

