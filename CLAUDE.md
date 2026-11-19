# Instructions for Claude sessions

This repo is the **data drop** for the MNQ bot. The code and all project docs live in
`johncombellick-cell/tradingsetup` (branch `claude/futures-trading-bot-t06mfa`, folder `ibkr-mnq-bot/`).
Read `ibkr-mnq-bot/docs/VERSION_X.md` there before doing a Version X review.

- Never commit secrets here. Only the Pi writes `daily/` (it regenerates days from its database); Claude sessions never
  edit `daily/` or `decisions/` — they are the record.
- Analyse the CSVs with Python and read only printed summaries; never print raw files into the conversation (tokens).
- Reviews write only `reviews/YYYY-MM-DD.json` (format in VERSION_X.md).
