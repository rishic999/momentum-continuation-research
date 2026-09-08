# Research charter: momentum continuation after a large run

## 1. The precise question

For a **liquid U.S. common stock** that has already made a large upward move, do point-in-time signals from business fundamentals, market expectations, price/volume behavior, peers, and the market regime improve our ability to estimate whether the stock will achieve a further upside target before suffering a defined drawdown?

The initial decision problem is deliberately framed as a competing-risk outcome:

> Conditional on a qualifying run-up at date *t*, what is the probability that the stock reaches **+20%** before **-10%** during the next **60 trading days**?

Those thresholds are research parameters, not trading rules. We will repeat the analysis across a pre-specified grid of targets, stops, and horizons.

## 2. Why this question

An investor often encounters a stock after the first dramatic repricing. Conventional momentum research says that return continuation can exist on average; earnings research says markets may adjust gradually to earnings news and forecast revisions. Neither statement directly answers the practical, conditional question: *is there still favorable payoff left after this particular run, given the information currently available?*

The project tests whether a transparent, diversified evidence set improves that conditional estimate. It does not assume that the answer is yes.

## 3. Unit of analysis and universe

- **Unit:** a stock-date event, not a company narrative and not a single famous winner.
- **Universe:** U.S.-listed common equities with minimum price and liquidity thresholds, including delisted securities where data permits.
- **Decision date:** the first market close after all required information is publicly available.
- **Study period:** to be fixed before data collection; target at least two full market cycles.

## 4. Initial event definition

An event occurs when, at the decision date:

1. trailing six-month total return is at least +75%;
2. the stock is above its 200-day moving average;
3. average daily dollar volume meets the pre-registered liquidity floor; and
4. it has not already been selected for the same event window.

This is a starting definition, not a result. Alternative definitions must be specified before testing, not selected after seeing performance.

## 5. Primary outcome

For each event, observe forward adjusted-close prices for 60 trading days:

- **Continuation:** +20% is reached before -10%.
- **Failure:** -10% is reached before +20%.
- **Unresolved:** neither barrier is reached within the horizon.

We will also report time to each barrier, forward return, maximum adverse excursion, maximum favorable excursion, and results around the next earnings announcement.

## 6. Hypotheses

### H1 — earnings expectations still matter

Continuation is more likely after a positive earnings/guidance surprise when forward earnings or revenue estimates are still being revised upward.

### H2 — quality of the trend matters

Continuation is more likely when the advance has broad participation, sustained relative strength, and constructive consolidation rather than a single unstable spike.

### H3 — confirmation matters

Continuation is more likely when industry peers and the relevant economic theme also exhibit positive relative strength and estimate revisions.

### H4 — risk regime changes payoff

Market stress, high volatility, sharp market rebounds after declines, and concentrated/crowded conditions worsen continuation outcomes or increase left-tail risk.

The null for each hypothesis is important: none of these signals improves out-of-sample calibration or economic results after realistic costs.

## 7. Scope guardrails

We will not:

- claim to predict the future of an individual company;
- use data revised after the decision date as if it had been known then;
- use a single-stock case study as evidence;
- tune feature definitions, horizons, or thresholds until a desired result appears;
- introduce options, transcripts, or complex ML before price-and-earnings baselines are established.

## 8. Success and failure criteria

The project is useful only if it adds value beyond simple price momentum and post-earnings-surprise baselines in a final untouched test period.

Evidence of value requires all of the following:

1. improved probability calibration (Brier score and calibration plots);
2. better ranking/discrimination (AUC and top-versus-bottom score buckets);
3. economically meaningful, cost-aware payoff improvement; and
4. stability across periods, sectors, and reasonable pre-specified parameter variants.

If these conditions fail, the correct result is that the added complexity did not earn its place.

## 9. Deliverable

The final deliverable will be a reproducible report containing the data definitions, code, event counts, full-sample and walk-forward results, failures, limitations, and a clearly separated exploratory appendix.

