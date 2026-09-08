# Literature map: what is known and what remains

## Established building blocks

### 1. Intermediate-horizon price momentum

Jegadeesh and Titman (1993) documented that prior winners outperformed prior losers over roughly 3–12 month horizons, with part of the effect dissipating at longer horizons. This establishes an average continuation effect; it does **not** provide a clock for an individual stock after a large move.

- Jegadeesh, N., & Titman, S. (1993). *Returns to Buying Winners and Selling Losers*. [Journal of Finance](https://doi.org/10.1111/j.1540-6261.1993.tb04702.x)

### 2. Earnings momentum and post-earnings-announcement drift

PEAD research finds that prices have historically continued to drift following earnings news, consistent with incomplete immediate incorporation of earnings information. Chan, Jegadeesh, and Lakonishok show that past returns, standardized unexpected earnings, and analyst forecast revisions contain distinct information and that combinations can be stronger than one signal alone.

- Bernard, V., & Thomas, J. (1989). *Post-Earnings-Announcement Drift*. [Journal of Accounting Research record](https://ideas.repec.org/a/bla/joares/v27y1989ip1-36.html)
- Chan, L., Jegadeesh, N., & Lakonishok, J. (1996). *Momentum Strategies*. [Journal of Finance](https://doi.org/10.1111/j.1540-6261.1996.tb05222.x)

### 3. Reference-price and industry context

George and Hwang (2004) show that the 52-week high, a simple reference point, explains a large portion of conventional momentum profits. Industry momentum research separately motivates peer-relative features rather than treating a company as isolated.

- George, T., & Hwang, C. (2004). *The 52-Week High and Momentum Investing*. [Journal of Finance](https://doi.org/10.1111/j.1540-6261.2004.00695.x)
- Moskowitz, T., & Grinblatt, M. (1999). *Do Industries Explain Momentum?* [Journal of Finance](https://doi.org/10.1111/0022-1082.00146)

### 4. Crash risk and implementation

Momentum earns positive average returns but is exposed to severe, clustered losses. Daniel and Moskowitz find that crashes are associated with panic conditions, high volatility, and market rebounds. Practitioner work also emphasizes turnover, liquidity, capacity, and transaction costs.

- Daniel, K., & Moskowitz, T. (2016). *Momentum Crashes*. [Journal of Financial Economics](https://doi.org/10.1016/j.jfineco.2015.12.002)
- Tobias, A., Moskowitz, T., Israel, R., & Serban, L. (2017). *Implementing Momentum: What Have We Learned?* [AQR working paper](https://www.aqr.com/Insights/Research/Working-Paper/Implementing-Momentum-What-Have-We-Learned)

### 5. Recent multimodal research

Recent work applies machine learning to PEAD and adds technical and fundamental data. This makes feature-rich modeling feasible, but it heightens the need for strict temporal validation and an honest comparison with simple baselines.

- Lim, B., et al. (2020). *Capturing Dynamics of PEAD Using Genetic-Algorithm-Optimised Supervised Learning*. [arXiv](https://arxiv.org/abs/2009.03094)

## What the literature does not settle

1. **Individual-event duration:** portfolio evidence does not answer exactly how long a particular post-run trend remains viable.
2. **A trader-shaped payoff:** most papers predict average return, not “upside target before drawdown” at a defined horizon.
3. **Unified, interpretable conditioning:** the evidence is often tested in separate signal families rather than as a pre-registered continuation score.
4. **Modern theme/peer structure:** broad thematic moves may need peer and supply-chain confirmation beyond standard industry codes.
5. **Incremental value:** complex transcript, options, and ML signals must prove improvement beyond low-cost price, earnings, and revisions data.

## Our contribution

We will not claim to discover momentum. We will test a practical, transparent and falsifiable extension: an event-conditioned competing-risk model for continuation after a large run, evaluated against price-only and earnings-only baselines using only data actually available at the decision date.

