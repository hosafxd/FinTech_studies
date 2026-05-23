---
title: FinTech Studies — LLM-Ready Markdown Collection
description: Index of the quant-finance research notebooks converted to semantic, LLM-friendly markdown.
---

# FinTech Studies — LLM-Ready Markdown Collection

This folder is a fully self-contained, LLM-friendly version of the parent
`collection/` directory. Every Jupyter notebook has been converted to a single
markdown file with a semantic header (description + "when this is useful")
on top, code cells preserved as fenced blocks, base64-encoded image outputs
embedded inline, and interactive Plotly charts summarized in prose.

CSV datasets have been replaced by markdown summaries (shape, columns, head,
tail, descriptive statistics, and a mid-table sample). Original CSV files
remain untouched in `../collection/`.

## How to read this collection

Each document begins with a YAML-style frontmatter block:

```
---
title: ...
category: ...
topics: [...]
source_notebook: ...
---
```

…followed by a `## Description` and a `## When this material is useful`
section. Treat the frontmatter as a quick lookup table: it tells you whether
a document is the right reference for a given question before you read the
body.

---

## Stochastic Calculus & Math Foundations

Core mathematical machinery: stochastic processes, integration, and SDEs.

| Document | What it covers |
| --- | --- |
| [Itô's Lemma — Clearly and Visually Explained](itos_lemma.md) | Why dW² = dt and the extra ½ σ² term in the chain rule for stochastic processes |
| [Itô Integration](ito_integration.md) | Forward Riemann sums, Itô vs Stratonovich, quadratic variation |
| [Solving Stochastic Differential Equations](solving_stochastic_differential_equations.md) | GBM, OU, mean-reverting models, Euler-Maruyama discretization |
| [Brownian Motion](brownian_motion.md) | Wiener process construction, √t scaling, simulation |
| [Markov Chains](markov_chains.md) | Transition matrices, stationary distributions, regime switching |
| [The Markov Property](mp.md) | Is the future independent of the past? Empirical tests on returns |

## Options Pricing & Volatility

Derivatives pricing, hedging, and the volatility surface.

| Document | What it covers |
| --- | --- |
| [Monte Carlo Simulation vs Black-Scholes](montecarlo_blackshcoles.md) | Analytical formula vs simulation, convergence, accuracy |
| [Why Monte Carlo Simulation Works](why_monte_carlo_simulation_works.md) | LLN + CLT, standard error, sample-size selection |
| [Trading with the Black-Scholes Model](Black-ScholesTrading.md) | Implied vol, Greeks, where the model breaks |
| [The Implied Volatility Surface](the_implied_volatility_surface.md) | Smile, skew, term structure, surface arbitrage checks |
| [Delta Hedging — Trading Strategy and Simulation](Delta_Hedging_Trading_Strategy.md) | Dynamic hedging P&L, gamma-theta tradeoff, discretization cost |

## Machine Learning & AI in Finance

Applying modern ML/DL to market data — and questioning whether it works.

| Document | What it covers |
| --- | --- |
| [What Does AI Actually Learn?](what_does_ai_actually_learn.md) | Interpretability, feature importance, overfitting diagnostics |
| [Neural Network Basics](neural_network_basics.md) | Perceptron, backprop, activations, gradient descent |
| [Neural Networks for Quant Finance](nn_for_quant/nn_quant.md) | Time-series-aware splits, architecture choice, feature engineering |
| [Time Series Analysis for Quant Finance](time_series_analysis_for_quant_finance.md) | Stationarity, ARIMA, GARCH, vol clustering, fat tails |

## Portfolio Management & Risk

Position sizing, drift estimation, and the statistics of trading.

| Document | What it covers |
| --- | --- |
| [Why Portfolio Optimization Doesn't Work](portfolio_optimization.md) | Markowitz sensitivity to estimation error, robust alternatives |
| [Expected Stock Returns Don't Exist](expected_returns_dont_exist.md) | Why estimating drift from history is essentially hopeless |
| [How to Trade with the Kelly Criterion](how_to_trade_with_the_kelly_criterion.md) | Optimal bet sizing, fractional Kelly, super-Kelly ruin |
| [Gambler's Ruin in Quant Trading](<gamblers_ruin_in_quant_trading(1).md>) | Ruin probability, bankroll math, absorbing states |
| [Is Trading Gambling?](is_trading_gambling.md) | Edge, expected value, LLN — the quantitative line |
| [When to Stop Trading a Profitable Strategy](When_to_Stop_Trading_a_Profitable_Strategy.md) | Strategy decay, kill-switches, Bayesian edge updates |
| [Problems with Statistics in Trading](Problems_with_Statistics_in_Trading.md) | p-hacking, multiple testing, look-ahead, survivorship bias |

## Market Data (CSV summaries)

Lightweight markdown summaries of the raw CSV datasets used by the notebooks.

| Document | What it covers |
| --- | --- |
| [NVDA — NVIDIA Historical Returns](data/NVDA_returns.md) | Shape, head, tail, descriptive stats for the NVDA OHLCV series |
| [SPX — S&P 500 Historical Returns](data/spx_returns.md) | Shape, head, tail, descriptive stats for the SPX OHLCV series |

## Reference images (standalone)

Diagrams that live outside any single notebook.

| Document | What it covers |
| --- | --- |
| [Markov-chain diagrams](standalone_images/README.md) | `chain_11.png`, `chain_22.png` — state-transition graphs |
| [Neural-network diagrams](nn_for_quant/images/README.md) | Network topology, train/val/test split, analogy figures |

---

## Topic index (quick lookup)

If you know the concept you need, here is the shortest path to the right doc:

- **Itô's lemma / SDE derivation** → [itos_lemma.md](itos_lemma.md)
- **Brownian motion simulation** → [brownian_motion.md](brownian_motion.md)
- **Solving an SDE numerically** → [solving_stochastic_differential_equations.md](solving_stochastic_differential_equations.md)
- **Markov property of prices** → [mp.md](mp.md), [markov_chains.md](markov_chains.md)
- **Pricing a European option** → [montecarlo_blackshcoles.md](montecarlo_blackshcoles.md), [Black-ScholesTrading.md](Black-ScholesTrading.md)
- **Why Monte Carlo converges** → [why_monte_carlo_simulation_works.md](why_monte_carlo_simulation_works.md)
- **Implied vol smile / skew** → [the_implied_volatility_surface.md](the_implied_volatility_surface.md)
- **Delta-hedging P&L** → [Delta_Hedging_Trading_Strategy.md](Delta_Hedging_Trading_Strategy.md)
- **Mean-variance pitfalls** → [portfolio_optimization.md](portfolio_optimization.md)
- **Estimating expected return** → [expected_returns_dont_exist.md](expected_returns_dont_exist.md)
- **Position sizing / leverage** → [how_to_trade_with_the_kelly_criterion.md](how_to_trade_with_the_kelly_criterion.md)
- **Probability of ruin** → [gamblers_ruin_in_quant_trading(1).md](<gamblers_ruin_in_quant_trading(1).md>)
- **Edge vs gambling** → [is_trading_gambling.md](is_trading_gambling.md)
- **Kill-switch / strategy decay** → [When_to_Stop_Trading_a_Profitable_Strategy.md](When_to_Stop_Trading_a_Profitable_Strategy.md)
- **Backtest sanity checks** → [Problems_with_Statistics_in_Trading.md](Problems_with_Statistics_in_Trading.md)
- **Neural-network primer** → [neural_network_basics.md](neural_network_basics.md), [nn_for_quant/nn_quant.md](nn_for_quant/nn_quant.md)
- **ML interpretability** → [what_does_ai_actually_learn.md](what_does_ai_actually_learn.md)
- **ARIMA / GARCH** → [time_series_analysis_for_quant_finance.md](time_series_analysis_for_quant_finance.md)

---

## Generation notes

- 22 notebooks converted via a stdlib-only `.ipynb` → `.md` script.
- Image outputs from notebooks are inlined as base64 `data:image/png;base64,...` URIs.
- Plotly interactive charts (no static image fallback) are replaced by a textual summary listing the chart title, axes, and trace names/types/lengths.
- Jupyter widget outputs are noted as non-renderable.
- CSV files are summarized to keep the LLM context budget manageable; full files remain in `../collection/`.
