# Crypto Trend Desk (scalping and intraday)

Open `index.html` in a browser (Chrome recommended). No install, no server. Needs internet for Binance, CoinGecko, news and TradingView.

Pages: Signals (index), Chart, Analysis, TradingView, Sessions, CPI, US jobs, Fed rates, US news, World news, Alerts.

- Timeframes: 5m, 15m, 1H, 4H shown. Daily is hidden but still used for the trend bias. Weekly removed.
- Coins: only market cap above $50M (CoinGecko), stablecoins excluded.
- Chart: HH/HL (uptrend) and LH/LL (downtrend) labels, support/resistance, breaks, retests, false breaks, retracement zone, candle patterns, last 50 and 100 candle shading.
- Signal: bigger trend (4H, 1H, daily) must agree, price at a pullback / retest / trap / breakout zone, confirming 5m or 15m candle, last 50 and 100 candle read, news window check. Stops use structure, targets 1R/2R/3R.
- News: CPI, jobs and Fed pages have editable numbers (pre-filled values may be outdated, verify). Event dates are in `js/macro.js`.
- TradingView: widget on the TradingView page, plus `pine/trend-desk-structure.pine` to paste into the Pine Editor.
- Alerts only fire while the Signals page is open. Optional Telegram.

Not financial advice. Test on paper first.

New: 4H levels are confirmed on the 15m chart and 1H levels on the 5m chart (reversal or trend break). Order blocks, breaker blocks, FVG, BOS/CHoCH, liquidity sweeps, equal highs/lows and 16 chart patterns are marked and used in the signal. Each signal shows its timeframe.

Backtest page (backtest.html): downloads real Binance history in your browser and replays the signal engine candle by candle.
