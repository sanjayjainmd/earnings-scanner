# Earnings Options Scanner

A single-page browser tool that screens stocks heading into earnings and flags whether a near-term options trade looks worth considering.

For each ticker it pulls live quote, price-history and options-chain data from Yahoo Finance and summarizes:

- **Expected move** implied by at-the-money option prices
- **Implied vs. historical volatility** (IV/HV ratio), to tell whether options are cheap or expensive
- **Earnings beat rate** over recent quarters and estimate revisions
- **Sector and market context** (sector ETF and SPY moves)

Each name is labeled **🟢 Call**, **🔴 Put**, or **🟡 Skip**, with an expandable detail view.

## Running it

No install or build step. Open `index.html` in a browser, enter tickers (or use the built-in list), and click **Scan**.

## Tech

Plain HTML, CSS and JavaScript in one file. Data requests go through public CORS proxies, so the page works with no backend.

*Personal research tool. Not investment advice.*
