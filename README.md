# 📒 Trading Journal

A fully offline, single-file trading journal built with vanilla HTML, CSS, and JavaScript. Designed for crypto paper traders who want to track trades, analyse patterns, and learn from mistakes — with no backend, no login, and no internet required after the first load.

**Live demo:** https://mustafa078.github.io/trading-journal/

---

## Features

### Trade Logging
- Log every trade with pair, direction, timeframe, entry / SL / TP
- Auto-calculated Risk:Reward ratio
- Risk % field with live dollar amount hint
- P&L tracking per trade
- Open trade status — log now, close later
- Attach a **chart screenshot** per trade (auto-compressed, stored locally)

### Tagging System
- **12 setup tags** — Liquidity Grab, Stop Hunt, BOS/MSS, Order Block, Fair Value Gap, EMA Bounce, Support Zone, Resistance Zone, Breakout, Trend Follow, Volume Profile, VWAP Bounce
- **8 emotion tags** — Confident, FOMO, Unsure, Calm, Greedy, Revenge, Bored, Patient
- **10 mistake tags** — Moved SL, Early/Late Entry, Chased Price, Ignored Plan, TP Too Early, No Clear Setup, Overleveraged, Revenge Trade, Wrong Context

### Stats Dashboard
- Total trades / Wins / Losses / Win rate
- Current streak tracker
- Net P&L with live balance update
- **Consecutive loss alert** — red warning banner triggers at 3+ losses in a row

### History
- Search trades by pair name
- Filter by result, open trades, mistakes, screenshots
- Edit any trade without deleting it
- One-click delete with confirmation

### Analytics (8 charts powered by Chart.js)
| Chart | What it shows |
|---|---|
| Emotion vs win rate | Which emotional state leads to best results |
| Win rate over time | Cumulative win rate as trades accumulate |
| Win rate by timeframe | Which TF (15M/1H/4H/1D) gives best entries |
| Win rate by day of week | Which days you trade most profitably |
| Setup performance | Win rate per strategy tag |
| Mistake analysis | Frequency + win rate impact of each mistake |
| Balance curve | Running balance over all closed trades |
| Pair breakdown | Per-pair trade count and win rate |

### Data & Persistence
- All data stored in **localStorage** — works fully offline
- **Export to JSON** — download a backup file anytime
- **Import from JSON** — restore data on any browser or device
- Starting balance locked on first launch (reset required to change)

---

## Tech Stack

- Pure HTML / CSS / JavaScript — no frameworks, no build tools
- [Chart.js](https://www.chartjs.org/) for analytics charts
- [Google Fonts](https://fonts.google.com/) — Inter + JetBrains Mono
- localStorage API for persistence
- Canvas API for screenshot compression

---

## Getting Started

No installation needed. Just open the file:

```bash
git clone https://github.com/mustafa078/trading-journal.git
cd trading-journal
# Open index.html in any browser
```

Or use the live version directly:
**https://mustafa078.github.io/trading-journal/**

---

## Usage

1. **First launch** — set your starting balance (locked until reset)
2. **Log trades** on the Log tab — fill in as much or as little as you want
3. **Tag setups and mistakes** honestly — the analytics only get useful with real data
4. **Close open trades** by clicking them in History
5. **Review Analytics** after 10+ trades to spot patterns
6. **Export a backup** regularly — go to History → Export

---

## Screenshots

> Coming soon

---

## Project Status

Active — built as a portfolio project and personal trading tool during paper trading practice.

---

## Author

**Muhammad Mustafa**
- GitHub: [@mustafa078](https://github.com/mustafa078)
