# Across Live Stream

Real-time dashboard for monitoring [Across Protocol](https://across.to) bridge deposits.

## What It Does

- **Deposits Monitor** (`index.html`) - Live table showing pending and filled bridge deposits with stats like fill rate, average fill time, and USD volume
- **Sankey Flow Diagram** (`sankey.html`) - Visual flow chart showing which chains are bridging to where in real-time

## Demo

Open `index.html` in your browser - no setup needed!

Both pages pull live data from the Across Protocol API and show token prices from CoinGecko.

## Features

- Live updates every 2 seconds
- Filter deposits by status (pending/filled)
- Highlights slow deposits that take longer than expected
- Shows USD value using real-time token prices
- Works on mobile

## Project Structure

```
across_live_stream/
├── index.html              # Main deposits monitor
├── sankey.html             # Flow visualization
└── assets/
    ├── chains/             # Chain logos (Ethereum, Base, etc.)
    ├── tokens/             # Token logos (ETH, USDC, etc.)
    ├── token_metadata.csv  # Token addresses and decimals
    └── token_prices_config.json  # CoinGecko token mappings
```

## Host It Yourself

Just upload everything to any static hosting:

- GitHub Pages
- Netlify
- Vercel
- Any web server

No backend needed - it's all client-side JavaScript.

## Credits
- Data: [Across Protocol API](https://across.to)
- Docs: [Across Protocol API Docs](https://docs.across.to/api-reference/introduction)

