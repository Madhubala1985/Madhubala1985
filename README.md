# Hi, I build quantitative trading systems 👋

I design and build **algorithmic trading platforms and quant research tooling**: real-time market-data
pipelines, options analytics, broker integrations, and the statistical machinery that decides whether
a strategy has a real edge *before* any capital is risked.

## 🔭 Featured projects

### 🥇 [XAU/USD Gold Quant Research Platform](https://github.com/Madhubala1985/xau-gold-quant-research)
Falsification-first research platform for spot gold. ~35k lines of Python, 850+ tests, MetaTrader 5 integration, and 7.5 years of M1 data.
- Pre-registered statistical gate: causal backtests, cost-stress grid, walk-forward k-fold, random-entry baselines (Bonferroni-corrected), out-of-sample holdout
- Tested every major Smart Money Concepts pattern, alone and combined
- **Result: a rigorous negative result.** No pattern beat random, so the system correctly stayed flat. The one shipped artifact is a macro regime risk dial.

### 📈 [Indian F&O Algo Trading v2](https://github.com/Madhubala1985/indian-fno-algo-trading-v2)
Autonomous NSE/BSE index-options system (Nifty, BankNifty, Sensex). ~92k lines and 213 commits.
- Ran every trading day on an Oracle Cloud VM against live Zerodha Kite data and real option prices, in fail-closed dry-run mode
- Options analytics: Greeks, IV surface, gamma exposure, dealer hedging, open interest
- Execution router behind 9 safety interlocks, a feed-stall watchdog, and reconciliation design
- **Result:** the dry run made +₹14,385 over 66 trades, but it was traced to a single day. I diagnosed the failure mode (bias staleness and long/short asymmetry) and **deliberately kept real funds disarmed**.

### 🧱 [Indian F&O Algo Trading v1](https://github.com/Madhubala1985/indian-fno-algo-trading-v1)
The foundation: an event-driven architecture (orchestrator, async event bus, dependency injection), WebSocket ingestion, multi-timeframe bar building, market-structure engines, backtesting, and paper trading for BankNifty.

## 🛠️ Toolbox
**Languages and core:** Python 3.12, asyncio, Pydantic, pandas, NumPy, scikit-learn, pytest
**Markets and brokers:** Zerodha Kite Connect, MetaTrader 5, NSE/BSE derivatives, XAU/USD
**Data and infra:** Redis, PostgreSQL/TimescaleDB, Oracle Cloud, systemd, Linux/WSL
**Quant methods:** walk-forward validation, Monte Carlo, cost/slippage modelling, options Greeks and GEX, regime models

## 💡 How I work
- **Prove the edge first, automate second.** Measure, don't assume.
- **Fail closed.** If a fill or a feed can't be confirmed, halt, never guess.
- **Report honestly.** A well-documented negative result beats a curve-fit backtest.

---
*Projects built with AI pair-programming (Claude Code). For research and education only. Not financial advice.*
