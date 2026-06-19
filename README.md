# Treasury Curve & Duration Hedging Workbench

A Python-based fixed-income analytics tool built in Google Colab.

## What It Does

- Downloads US Treasury constant-maturity yields (1M–30Y) from FRED (Federal Reserve)
- Bootstraps a zero-coupon curve from par yields
- Prices a stylised bond portfolio using real market yields
- Computes Macaulay duration, modified duration, DV01, and convexity
- Simulates portfolio P&L under parallel yield curve shifts (-200bp to +200bp)
- Constructs a DV01-neutral hedge overlay using Treasury ETFs (SHY, IEF, TLT)
- Measures hedge efficiency and compares hedged vs unhedged P&L

## Data Sources

- **FRED (Federal Reserve Economic Data)** — Treasury constant-maturity yields
- **Yahoo Finance (yfinance)** — Treasury ETF prices (SHY, IEF, TLT)

## Key Concepts Demonstrated

- Term structure and yield curve bootstrapping
- Bond pricing from yield to maturity
- Duration, modified duration, convexity, and DV01
- Parallel shift scenario analysis
- Single-factor DV01-neutral hedge construction
- Hedge effectiveness measurement

## Libraries Used

`pandas` · `numpy` · `plotly` · `yfinance` · `pandas_datareader`

## How to Run

1. Open in Google Colab
2. Run cells top to bottom
3. No API keys required

## Industry Relevance

Banks, insurers, and fixed-income portfolio managers use equivalent tooling
to monitor interest-rate exposure and immunise liability portfolios.
