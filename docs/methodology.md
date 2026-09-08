# Methodology

## Design principle

Every feature must have an availability timestamp. A row may only use data released at or before its decision timestamp. Revised fundamentals, restated results, later consensus estimates, and survivorship-filtered universes are prohibited from the production backtest.

## Baselines first

Before modeling, we will report unconditional event outcomes and compare against:

1. **Price-only baseline:** trailing return, distance to 52-week high, relative strength, realized volatility, and volume trend.
2. **Earnings baseline:** standardized earnings surprise, post-announcement abnormal return, guidance direction, and estimate-revision breadth.
3. **Combined interpretable model:** regularized logistic regression or monotonic gradient boosting with a small, documented feature set.

Complex models must beat these baselines in a later chronological period; otherwise they are not retained.

## Feature families

| Family | First-pass measures | Purpose |
|---|---|---|
| Price/trend | trailing returns, 52-week-high distance, moving-average distance, trend persistence | distinguish sustained trends from spikes |
| Volume/volatility | dollar-volume trend, realized volatility, downside volatility, gap behavior | measure participation and fragility |
| Earnings | standardized surprise, revenue surprise, guidance | measure new fundamental information |
| Revisions | 1/3-month estimate changes, breadth, dispersion | measure whether expectations continue to rise |
| Peers | industry relative strength/revisions, breadth | seek thematic confirmation |
| Regime | market trend, volatility, drawdown/rebound state | control known momentum crash states |

## Validation

- Split data chronologically into development, validation, and final untouched test periods.
- Purge/embargo overlapping forward-label windows between folds.
- Perform all transformations within each training window.
- Preserve delisted securities and use total-return adjustments where possible.
- Report confidence intervals by time-block bootstrap and results by decade, sector, and market regime.

## Metrics

Statistical metrics: event count, class rate, Brier score, calibration curve, AUC, precision/recall, and confidence intervals.

Economic metrics: target-before-stop rate, mean/median forward return, maximum adverse excursion, turnover, conservative trading costs, drawdown, and capacity/liquidity diagnostics.

The primary claim is conditional probability calibration—not the backtested Sharpe ratio.

