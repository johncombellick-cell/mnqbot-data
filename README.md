# mnqbot-data

Private data drop for the MNQ bot (code: `johncombellick-cell/tradingsetup`, folder `ibkr-mnq-bot/`).
**No secrets live here** — only prices, trades and review notes.

| Folder | Written by | Contents |
|---|---|---|
| `daily/YYYY-MM-DD/` | the Pi, ~16:10 ET each weekday (`scripts/backfill_data.py` regenerates past days) | **that day only**: `trades.csv` (all versions, real + shadow), `bars.csv` (1-min MNQ bars with volume/candle features), `signals.csv`, `runs.csv` |
| `market_days.csv` | the Pi, daily (replaced) | every day's regular-hours open/high/low/close + volatility stats |
| `history/` | the Pi, on request (`scripts/fetch_history.py`) | historical 1-min MNQ bars for screening Version X ideas (allowed for Version X only, user 2026-11-13) |
| `reviews/YYYY-MM-DD.json` | the daily Claude review, ~16:30 ET | the recommendation the Telegram bot sends at 16:45 |
| `decisions/YYYY-MM-DD.json` | the Pi, when the user taps Approve / Keep in Telegram | the user's decision on a proposed change |
