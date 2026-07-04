# West Heaton Poker League — Claude Instructions

## Points System

When given a month's results, apply this points scale:

| Position | Base | Bubble bonus | Total awarded |
|----------|------|--------------|---------------|
| 1st | 25 | – | 25 |
| 2nd | 20 | – | 20 |
| 3rd | 15 | – | 15 |
| 4th | 12 | – | 12 |
| 5th | 9 | +10 | **19** |
| 6th | 6 | – | 6 |
| 7th | 4 | – | 4 |
| 8th | 2 | – | 2 |

**5th is the bubble position** (last out before the money). They receive 9 base + 10 bonus = 19 total — intentionally more than 4th place (12).

## Input Format

Results are passed as a list in **finish-position order** (1st through 8th). The number next to each player's name is their correct final points total, already including the bubble bonus for 5th.

Example input:
```
25 - Player A   ← 1st place
20 - Player B   ← 2nd place
15 - Player C   ← 3rd place
12 - Player D   ← 4th place
19 - Player E   ← 5th place (bubble)
6  - Player F   ← 6th place
4  - Player G   ← 7th place
2  - Player H   ← 8th place
```

The 19 for 5th will always appear "out of order" by value — that is correct.

## Name Conventions

- Respect player name spellings exactly as given.
- "Chloi" is correct — do not change to "Chloe".
- "Helen B" and "Helen Dobson" are two different players.

## Adding a New Month

1. Add a new `### Month YYYY` section to `results.md` with the finish-order table.
2. Recalculate the Overall Standings table (add the new month's column and update totals).
3. Update the `months` list in the YAML frontmatter.
