# 🏉 Six Nations Fantasy Rugby 2026

## The Armchair Coaches

A simple, static fantasy rugby app for the Six Nations. Hosted free on GitHub Pages.

## How to Deploy

1. Create a GitHub repo
2. Drop `index.html` into the root
3. Enable GitHub Pages (Settings → Pages → Deploy from main branch)
4. Share the URL with your league!

## How Scoring Works

After each round, a `roundX.json` file is added with player stats.
The scoring engine in `index.html` calculates fantasy points automatically.

### Scoring Rules
| Action | Points |
|--------|--------|
| Try | +20 |
| Try assist | +10 |
| Conversion | +5 |
| Penalty goal | +3 |
| Drop goal | +10 |
| Clean break | +5 |
| Offload | +3 |
| Tackle | +1 |
| Turnover won | +7 |
| Lineout steal | +5 |
| Winning team | +5 |
| Captain | ×2 |
| MoM | +15 |
| Hat-trick | +10 |
| Missed tackle | −1 |
| Penalty conceded | −3 |
| Yellow card | −10 |
| Red card | −20 |

## Updating Scores

After each round:
1. Ask Metamate to process the match stats (paste Opta URLs or stats)
2. Metamate generates the `roundX.json` file
3. Upload to the repo
4. Site updates automatically!

## Team Rules
- 15 players (11 starting + 4 bench)
- €100m budget
- Max 5 players per nation
- 1 captain per round (points doubled)
- 2 free transfers per round (−5pts each extra)

