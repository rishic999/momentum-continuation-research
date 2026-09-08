# Data plan

## Phase 1: reproducible price-only prototype

| Need | Minimum data | Candidate source | Constraint |
|---|---|---|---|
| Prices, volume, corporate actions | daily adjusted OHLCV, delistings | CRSP (ideal) or an explicitly limited public source | avoid survivorship bias |
| Universe and classifications | exchange, share class, sector/industry | CRSP/Compustat or vendor mapping | timestamp changes where possible |
| Market regime | broad-index total returns and volatility proxy | public index data / FRED | document availability timing |

This phase can validate the event engine and labels but cannot answer the fundamental-information hypothesis.

## Phase 2: earnings and expectations

| Need | Preferred source | Why point-in-time matters |
|---|---|---|
| Actual earnings, announcement timestamp | Compustat / vendor event feed | eliminates date ambiguity |
| Consensus estimates and revisions | I/B/E/S or point-in-time vendor | later consensus snapshots cause leakage |
| Guidance and transcripts | licensed transcript provider / archived filings | need release-time availability |

## Phase 3: optional extensions

- Options-implied volatility, skew, open interest, and volume from a historical options vendor.
- Transcript NLP and management-language features.
- Supply-chain or custom thematic peer networks.

No extension is added unless its data availability, license, timestamp, and incremental out-of-sample value are documented.

## Data governance

Raw licensed data, API keys, and redistributable-restricted files never enter Git. The repository stores acquisition instructions, schema contracts, synthetic examples, transformations, and reproducible code.

