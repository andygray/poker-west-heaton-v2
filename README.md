# West Heaton Poker League 2026

Teletext-styled single-page leaderboard for the West Heaton monthly poker league.

## Stack

Static HTML + CSS + vanilla JS. No build step. Fonts served from [galax.xyz/TELETEXT](https://galax.xyz/TELETEXT/).

## Deployment

Hosted on Vercel. Push to `main` → auto-deploys.

```bash
npx vercel --prod   # manual deploy
```

## Adding a new month

1. Update `results.md` with the month's results (finish-position order, 1st–8th).
2. Update the Overall Standings table in `results.md`.
3. Add a new `<div id="month" class="page">` block in `index.html`.
4. Add a nav button in the `.nav` bar.

## Points system

| Position | Points | Note |
|----------|--------|------|
| 1st | 25 | |
| 2nd | 20 | |
| 3rd | 15 | |
| 4th | 12 | |
| 5th | 19 | Bubble: 9 base + 10 bonus |
| 6th | 6 | |
| 7th | 4 | |
| 8th | 2 | |

5th place is the bubble — last out before the money — and receives a +10 bonus, giving them more points than 4th.
