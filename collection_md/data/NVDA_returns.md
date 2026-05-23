---
title: NVDA (NVIDIA) Historical Returns
category: Market Data
source_csv: NVDA_returns.csv
---

# NVDA (NVIDIA) Historical Returns

> **Category:** Market Data  
> **Source CSV:** `NVDA_returns.csv`

## Description

Time-series of NVIDIA (NVDA) stock returns used as a single-name dataset across the notebooks (volatility modeling, IV-surface fitting, drift-estimation demos).

## When this dataset is useful

- Single-name return-series examples (Brownian/GBM fits, volatility estimation)
- Stress-testing models with a high-vol, high-skew real-world series
- Drift / Sharpe estimation demos where the answer is genuinely unstable
- Single-asset Kelly-criterion sizing exercises

---


## Shape

- Rows: **6,683**
- Columns: **7**

## Columns

- `Date` — *text/date*
- `Open` — *numeric*
- `High` — *numeric*
- `Low` — *numeric*
- `Close` — *numeric*
- `Adj Close` — *numeric*
- `Volume` — *text/date*

## Head (first 10 rows)

| Date | Open | High | Low | Close | Adj Close | Volume |
| --- | --- | --- | --- | --- | --- | --- |
| 5/27/2025 | 134.15 | 135.66 | 133.31 | 135.5 | 135.5 | 190,549,430 |
| 5/23/2025 | 130 | 132.68 | 129.16 | 131.29 | 131.29 | 198,367,700 |
| 5/22/2025 | 132.23 | 134.25 | 131.55 | 132.83 | 132.83 | 187,344,000 |
| 5/21/2025 | 133.06 | 137.4 | 130.59 | 131.8 | 131.8 | 270,608,700 |
| 5/20/2025 | 134.29 | 134.58 | 132.62 | 134.38 | 134.38 | 161,514,200 |
| 5/19/2025 | 132.39 | 135.87 | 132.39 | 135.57 | 135.57 | 193,154,600 |
| 5/16/2025 | 136.22 | 136.35 | 133.46 | 135.4 | 135.4 | 226,542,500 |
| 5/15/2025 | 134.29 | 136.3 | 132.66 | 134.83 | 134.83 | 226,632,600 |
| 5/14/2025 | 133.2 | 135.44 | 131.68 | 135.34 | 135.34 | 281,180,800 |
| 5/13/2025 | 124.98 | 131.22 | 124.47 | 129.93 | 129.93 | 330,430,100 |

## Tail (last 10 rows)

| Date | Open | High | Low | Close | Adj Close | Volume |
| --- | --- | --- | --- | --- | --- | --- |
| 2/4/1999 | 0.04 | 0.04 | 0.04 | 0.04 | 0.04 | 181,920,000 |
| 2/3/1999 | 0.04 | 0.04 | 0.04 | 0.04 | 0.03 | 75,120,000 |
| 2/2/1999 | 0.04 | 0.04 | 0.04 | 0.04 | 0.03 | 264,096,000 |
| 2/1/1999 | 0.04 | 0.04 | 0.04 | 0.04 | 0.04 | 154,704,000 |
| 1/29/1999 | 0.04 | 0.04 | 0.04 | 0.04 | 0.04 | 244,032,000 |
| 1/28/1999 | 0.04 | 0.04 | 0.04 | 0.04 | 0.04 | 227,520,000 |
| 1/27/1999 | 0.04 | 0.04 | 0.04 | 0.04 | 0.04 | 244,368,000 |
| 1/26/1999 | 0.05 | 0.05 | 0.04 | 0.04 | 0.04 | 343,200,000 |
| 1/25/1999 | 0.04 | 0.05 | 0.04 | 0.05 | 0.04 | 510,480,000 |
| 1/22/1999 | 0.04 | 0.05 | 0.04 | 0.04 | 0.04 | 2,714,688,000 |

## Descriptive statistics (numeric columns)

| statistic | Open | High | Low | Close | Adj Close |
| --- | --- | --- | --- | --- | --- |
| count | 6627 | 6627 | 6627 | 6627 | 6627 |
| mean | 9.922629 | 10.108711 | 9.718569 | 9.923041 | 9.895598 |
| std | 26.240628 | 26.7259 | 25.678155 | 26.224972 | 26.226307 |
| min | 0.03 | 0.04 | 0.03 | 0.03 | 0.03 |
| 25% | 0.28 | 0.29 | 0.27 | 0.28 | 0.26 |
| 50% | 0.47 | 0.48 | 0.46 | 0.47 | 0.44 |
| 75% | 4.92 | 4.98 | 4.83 | 4.92 | 4.88 |
| max | 153.03 | 153.13 | 147.82 | 149.43 | 149.42 |

## Random sample (5 rows from the middle)

| Date | Open | High | Low | Close | Adj Close | Volume |
| --- | --- | --- | --- | --- | --- | --- |
| 4/26/2012 | 0.33 | 0.33 | 0.32 | 0.33 | 0.3 | 539,208,000 |
| 4/25/2012 | 0.33 | 0.33 | 0.32 | 0.33 | 0.3 | 727,112,000 |
| 4/24/2012 | 0.33 | 0.33 | 0.32 | 0.32 | 0.29 | 730,440,000 |
| 4/23/2012 | 0.33 | 0.33 | 0.32 | 0.33 | 0.3 | 706,244,000 |
| 4/20/2012 | 0.34 | 0.34 | 0.33 | 0.33 | 0.31 | 509,592,000 |
