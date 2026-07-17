# QuantTerminal: Financial Analytics & Backtesting Engine

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![SciPy](https://img.shields.io/badge/SciPy-Optimization-8CAAE6)
![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Charts-3F4F75)
![License](https://img.shields.io/badge/License-MIT-green)

QuantTerminal is a simplified, personal version of a professional financial research terminal. It lets a user search any listed company, pull up financial statements, analyze and compare stock performance, screen stocks by financial metrics, track economic indicators, optimize multi-asset portfolios, measure risk, and backtest systematic trading strategies — all in one Python-based environment.

<!-- Add a screenshot or GIF of the dashboard here -->
<!-- ![QuantTerminal Dashboard](path/to/screenshot.png) -->

## Features

- **Company Search** — Look up any listed company by ticker and pull its core profile and financials.
- **Financial Statements** — View income statement, balance sheet, and cash flow data.
- **Stock Performance Analysis** — Historical price trends, returns, and volatility for any ticker.
- **Company Comparison** — Compare multiple companies side by side on key financial metrics.
- **Stock Screener** — Filter and rank stocks based on financial metrics (e.g., P/E, market cap, revenue growth).
- **Economic Indicator Tracking** — Monitor macro indicators (e.g., interest rates, inflation, GDP) alongside market data.
- **Portfolio Optimization** — Mean-variance optimization (`SciPy`) to compute the Maximum Sharpe Ratio portfolio.
- **Risk Analytics** — Historical Value at Risk (VaR) and rolling volatility profiling.
- **Vectorized Backtesting** — Fast, event-free simulation of strategies (e.g., SMA crossovers) with no look-ahead bias.
- **Interactive Dashboards** — Plotly-based visualizations across all of the above.

## Backtest Results

<!-- Fill this in once you run a backtest -->

| Strategy | Total Return | Sharpe Ratio | Max Drawdown | Benchmark (Buy & Hold) |
|---|---|---|---|---|
| SMA Crossover (50/200) | | | | |

## Tech Stack

| Category | Tools |
|---|---|
| Language | Python |
| Data Processing | Pandas, NumPy |
| Quant Modeling | SciPy |
| Visualization | Plotly |
| Data Source | Yahoo Finance (`yfinance`) |

## Getting Started

### Option 1: Google Colab (no setup)
1. Open [Google Colab](https://colab.research.google.com/).
2. Upload or open the project notebook.
3. Run the setup cell:
   ```
   !pip install yfinance plotly scipy pandas numpy
   ```
4. Run the pipeline to generate the dashboard.

### Option 2: Local Setup
```bash
git clone https://github.com/<your-username>/QuantTerminal.git
cd QuantTerminal
pip install -r requirements.txt
python main.py
```

## Project Structure

```
QuantTerminal/
├── quantterminal/
│   ├── data_pipeline.py      # Data ingestion, financials, economic indicators
│   ├── screener.py           # Stock screening by financial metrics
│   ├── optimizer.py          # Portfolio optimization
│   └── backtester.py         # Vectorized backtesting engine
├── notebooks/
│   └── quantterminal_demo.ipynb
├── requirements.txt
└── README.md
```

## Core Modules

- **`QuantDataPipeline`** — Handles API calls, company financials, missing data, and log return calculations.
- **`StockScreener`** — Filters and ranks companies against user-defined financial criteria.
- **`PortfolioOptimizer`** — Minimizes negative Sharpe ratio subject to weight constraints.
- **`VectorizedBacktester`** — Generates trading signals and computes cumulative strategy returns against a benchmark.

## Author

**Shashwat Rai**
B.Tech Electronics & Communication Engineering (ECE)
Interested in quantitative development and building analytical systems that turn raw market data into decision-ready insight.

## License

MIT License — see [LICENSE](LICENSE) for details.
