### Jonas Löffler — volatility, options & honest backtesting

I study **volatility**: how to forecast it, how options price it, and how to tell a real trading edge from an overfit one.

→ **[Website](https://jonaslffr-ship-it.github.io/)** — my research plus seven interactive tools: live SPX volatility from Cboe delayed data, a 3D volatility surface, option greeks, dealer gamma, 0DTE variance, realized vol and a backtest lab

**Research**
- **Realized-volatility forecasting on the S&P 500** (working paper v1.1; 21 years of 1-minute data) — implied volatility adds forecast information beyond HAR (Clark–West p = 0.019); my best volatility-managed strategy was disqualified by my own pre-registered rules (PBO = 0.84). *Public release in preparation.*
- **Same-day implied variance from 0DTE S&P 500 options, 2018–2026** *(in progress — pre-registration first)* — how much volatility the market prices for a single trading day, and whether that price is fair.

**Interactive tools** (dark-mode web app, everything runs in the browser)
- **[Live SPX volatility](https://jonaslffr-ship-it.github.io/#live)** — today’s implied-vol surface (SVI per expiry, bid–ask fit quality), model-free implied moves checked against the VIX, dealer-gamma scenarios, moneyness and a history-and-live chart of SPX and the VIX family — rebuilt every 30 minutes from Cboe delayed data by a GitHub Action
- **[Volatility surface](https://jonaslffr-ship-it.github.io/#surface)** — SSVI in 3D with butterfly/calendar arbitrage checks, Dupire local vol and the implied density
- **[Options & Greeks](https://jonaslffr-ship-it.github.io/#greeks)** — strategy builder; P&L and 13 greeks to third order as 3D surfaces, each checked live against a finite difference
- **[Dealer Gamma Lab](https://jonaslffr-ship-it.github.io/#dealer)** — why dealer long gamma dampens moves and short gamma amplifies them: derived, simulated, and explicit about the identification problem
- **[Overfitting simulator](https://jonaslffr-ship-it.github.io/#backtest)** — CSCV / probability of backtest overfitting and the deflated Sharpe ratio
- **[The Sharpe-8 illusion](https://jonaslffr-ship-it.github.io/#backtest)** — how bar backtests invent profits that tick data takes away
- **[Realized vol](https://jonaslffr-ship-it.github.io/#realized)** — which range estimator to trust, and a HAR forecasting lab with a Diebold–Mariano test
- **[0DTE variance](https://jonaslffr-ship-it.github.io/#odte)** — Cboe variance replication on a synthetic 0DTE chain, implied and event-day moves

**Teaching**
- **[Trading Library](https://github.com/jonaslffr-ship-it/trading-library)** — 22 original papers across seven tracks; every number reproducible from free data

`HAR / HAR-IV` · `QLIKE · Diebold–Mariano · Clark–West · MCS` · `deflated Sharpe · PBO/CSCV` · `Black–Scholes greeks to 3rd order` · `model-free implied variance` · `Python (pandas, NumPy, SciPy, statsmodels)`

Research standards: pre-registration first · out of sample, or it didn't happen · errata, not silent edits.
