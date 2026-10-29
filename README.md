# Observe Profit Charts ($OPC)

Single-file site: `index.html` (no build step, no folders). Deploy as-is on Vercel or GitHub Pages.

## Set your links
Near the top of the script in `index.html`:

```js
var CONFIG={xUrl:'',xHandle:'',ca:'',buyUrl:''};
```

Add or remove listed tokens in `MINTS` (Solana mint addresses).

## Data
- Live prices, market cap, 24h volume, 24h change and pool liquidity: DexScreener public API (refreshed every 30s).
- Live 1h candles on the Observe chart: GeckoTerminal public API.
- "Chart impact" is a constant-product estimate from total pool liquidity.
- If the APIs can't be reached, the page shows a labelled snapshot.

## Preview features
- Open offers are samples priced off live spot.
- Make offer / Positions and Add a bag save to the visitor's browser.
- Look up any wallet opens Solscan.
- Signing, escrow and settlement are planned for launch.
