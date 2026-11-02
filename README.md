# ☘ Luck Society · Smart Money Scanner

Live open-position scanner for Polymarket's most profitable **non-sports** traders: politics, elections, geopolitics, economy, finance, crypto, tech, culture, weather and mentions markets.

Hit **SCAN** and the page pulls every open bet from the tracked roster straight from Polymarket's public API — no server, no keys.

Sister site: [Sharp Money Scanner](https://lucksociety.github.io/polymarket-sharp-scanner/) (sports).

## What it shows
- **By resolution date:** Awaiting Resolution → Resolves Today → Tomorrow → each day this week → Next 30 Days → Next 3 Months → This Year → Long-Dated, each collapsible
- **Conviction:** every bet's value as a % of that trader's open book — 🔥 Max (10%+), High (4–10%), Med (1–4%), Low (<1%). Accounts under $25K are capped at Med.
- **Biggest Conviction Plays:** the 8 bets resolving within 30 days that are the largest share of a trader's book
- **Smart Consensus:** markets where 2+ tracked traders are on the same side
- **Hedge filter:** hides bets where a trader holds both sides of a market (usually market-making)
- **Category tabs:** Elections, Politics, Geopolitics, Economy, Finance, Crypto, Tech, Culture, Weather, Mentions, Other (sports hidden unless you tick "Include sports")
- **+ Hot hands:** also scans this month's top traders on the Politics, Crypto, Economics, Finance, Tech, Culture, Weather and Mentions leaderboards

## The roster
32 traders who are **active** (traded in the last 30 days), have **$100K+ lifetime non-sports profit**, and make little or nothing on sports. The biggest all-time names (Theo4, Fredi9999, zxgngl, etc.) are left out because they haven't traded since the 2024 election and hold nothing.

Edit the `CORE` list near the top of the `<script>` in `index.html` to change it:

```js
{ name:"elmcap2", wallet:"0xed107a85a4585a381e48c7f7ca4144909e7dd2e5", spec:"Economics · Politics" },
```

## Data sources
- Positions: `data-api.polymarket.com/positions`
- Open book value: `data-api.polymarket.com/value`
- Leaderboards: `data-api.polymarket.com/v1/leaderboard`
- Categories: `gamma-api.polymarket.com/events` tags

Not betting advice. Big P&L can come from market-making, insider-ish edges or a single lucky hit — do your own homework.
