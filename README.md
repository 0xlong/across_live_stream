# Across Live Stream

Real-time dashboard for monitoring Across Protocol bridge deposits - [Live Dashboard](https://0xlong.github.io/across_live_stream/)

## What It Does

- **Deposits Monitor** (`index.html`) - Live table showing pending and filled bridge deposits (relays) with stats like fill rate, average fill time, and USD volume calculated per minute
- **Sankey Flow Diagram** (`sankey.html`) - Visual flow chart showing which chains are bridging to where in real-time by volume as edge size and flying dot is a live transaction happening :)

Both pages pull live data from the Across Protocol API and show token prices from CoinGecko.

## Features

- Live updates every 2 seconds
- Filter deposits by status (pending/filled)
- Highlights slow deposits (> 60s) at the top of the page to take action if realy is pending for too long
- Shows USD value using real-time token prices
- pending transactions alerts can be sent automatically to notify team to take care of transactions that are taking too long to process

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

