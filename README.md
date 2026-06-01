# Fantasy Rugby Six Nations 2026 — "The Armchair Coaches"

A single-page Fantasy Rugby web app for the 2026 Six Nations Championship.  
Built as one `index.html` file (~41KB) for GitHub Pages. No external dependencies — pure HTML/CSS/JS.

---

## Quick Start

1. Copy `index.html` to your GitHub Pages repository
2. Push to deploy
3. Share the URL with your league members
4. Admin manages data via `yoursite.github.io/#admin`

---

## How It Works

- **Squad**: Each manager picks 23 players (15 starting + 8 bench) within a €100m budget
- **Limits**: Max 5 players per nation
- **Captain**: 1 captain per round (scores ×1.5)
- **Transfers**: 2 free transfers per round; additional transfers cost -5pts each
- **Bench**: Bench players earn half points
- **Lock**: All teams lock at the **first kickoff of the round** — no changes after that

---

## Player Database

The app includes **138+ players** (23-man matchday squad × 6 nations per round).  
Over the course of the tournament, the total pool grows as coaches make changes between rounds — expect **150–170 unique players** across all 5 rounds.

Players are priced from €5m (bench props) to €12m (premium players like Dupont), based on form and quality.

---

## Scoring Rules

| Action | Points |
|--------|--------|
| Try | +20 |
| Try Assist | +10 |
| Conversion | +3 |
| Penalty Goal | +3 |
| Drop Goal | +10 |
| Clean Break | +5 |
| Offload | +3 |
| Metres Made | +0.1 per metre |
| Defenders Beaten | +1 |
| Tackle | +1 |
| Turnover Won | +7 |
| Lineout Steal | +5 |
| Winning Team | +5 |
| Man of the Match | +15 |
| Hat-trick Bonus | +10 |
| Missed Tackle | -1 |
| Penalty Conceded | -3 |
| Yellow Card | -10 |
| Red Card | -20 |
| **Captain** | **×1.5** |
| **Bench players** | **Half points** |

---

## Admin Instructions — Round-by-Round Workflow

You (the league admin) need to do a few things each round. Here's the step-by-step:

### 📋 Step 1: Update Team Sheets (~48 hours before first kickoff)

**When:** Teams are officially announced ~48 hours before kickoff.  
- For Saturday matches → announced **Thursday lunchtime**  
- For Friday matches → announced **Wednesday lunchtime**  
- For Sunday matches → announced **Friday lunchtime**  

**Where to find them:**
1. [sixnationsrugby.com](https://www.sixnationsrugby.com) — consolidated team sheets
2. National union sites: [irishrugby.ie](https://www.irishrugby.ie), [ffr.fr](https://www.ffr.fr), [scottishrugby.org](https://www.scottishrugby.org), [englandrugby.com](https://www.englandrugby.com), [wru.wales](https://www.wru.wales), [federugby.it](https://www.federugby.it)
3. [BBC Sport Rugby](https://www.bbc.co.uk/sport/rugby-union) — usually within minutes of announcement

**What to do:**
1. Go to `yoursite.github.io/#admin`
2. Create/update the **team sheets JSON** for the round (see format below)
3. Paste it into the Admin panel textarea and click **Load Data**
4. This updates the player database so managers can see who's starting/benched
5. Verify the player list looks correct in the Transfer Market tab

> ⚡ **Tip:** Check again on match morning — late changes occasionally happen after the captain's run (usually just injury-forced swaps on the bench).

### 🔒 Step 2: Confirm Lock Time

**When:** The app automatically locks all teams at the **first kickoff of the round**.

| Round | Lock Time (First Kickoff) |
|-------|--------------------------|
| 1 | Thu 5 Feb 2026, 20:10 GMT |
| 2 | Sat 14 Feb 2026, 14:10 GMT |
| 3 | Sat 21 Feb 2026, 14:10 GMT |
| 4 | Fri 6 Mar 2026, 20:10 GMT |
| 5 | Sat 14 Mar 2026, 14:10 GMT |

**What to do:**
1. In the Admin panel, confirm the **round deadline** is set correctly
2. The countdown timer on the main page will show managers how long they have left
3. Once locked, managers cannot make transfers or change their captain
4. Remind the league in your group chat: _"Teams lock at [TIME] — get your transfers in!"_

### 📊 Step 3: Enter Match Results & Scoring (after all games complete)

**When:** After the final whistle of the last match in the round (typically Saturday evening / Sunday).

**Where to get scoring data:**
1. **Match results & try scorers**: [sixnationsrugby.com](https://www.sixnationsrugby.com) → Match Centre
2. **Detailed stats** (tackles, carries, offloads, metres): [rugbypass.com](https://www.rugbypass.com) → Match Stats (Opta-powered)
3. **Man of the Match**: Usually announced on broadcast / sixnationsrugby.com
4. **Kicking stats** (conversions, penalties): Match Centre on sixnationsrugby.com

**What to do:**
1. Go to `yoursite.github.io/#admin`
2. Create the **round results JSON** (see `roundX.json` format below)
3. For each match, record:
   - Final score
   - Try scorers (and minute)
   - Try assists (if available)
   - Conversions and penalties kicked (and by whom)
   - Yellow/red cards
   - Man of the Match
   - Detailed player stats (if sourcing from RugbyPass)
4. Paste the JSON into Admin panel and click **Load Data**
5. The scoring engine will automatically calculate points for all players
6. Check the League Table updates correctly

> ⚡ **Tip:** Start with tries + kicking + cards + MoM (the big point-scorers). Add detailed stats (tackles, metres, offloads) later if you have time — they're smaller point values.

### 🔄 Step 4: Open Next Round for Transfers

**When:** After scoring is loaded and verified.

**What to do:**
1. Update the player database with any new squad members (injury replacements, etc.)
2. Set the next round's deadline in the Admin panel
3. Managers can now start making their 2 free transfers for the next round
4. Post in the group chat: _"Round X scores are in! Transfers open for Round Y."_

---

## Round Data JSON Format

### Team Sheets (pre-round)

```json
{
  "round": 1,
  "deadline": "2026-02-05T20:10:00Z",
  "team_sheets": [
    {
      "team": "France",
      "starting_xv": [
        {"number": 1, "name": "Jean-Baptiste Gros", "position": "PR"},
        {"number": 2, "name": "Julien Marchand", "position": "HK"}
      ],
      "replacements": [
        {"number": 16, "name": "Peato Mauvaka", "position": "HK"}
      ]
    }
  ]
}
```

### Match Results (post-round)

```json
{
  "round": 1,
  "matches": [
    {
      "home": "France",
      "away": "Ireland",
      "home_score": 36,
      "away_score": 14,
      "venue": "Stade de France, Paris",
      "mom": "Louis Bielle-Biarrey"
    }
  ],
  "player_stats": [
    {
      "name": "Louis Bielle-Biarrey",
      "team": "France",
      "tries": 2,
      "conversions": 0,
      "penalties": 0,
      "clean_breaks": 3,
      "tackles": 4,
      "turnovers_won": 0,
      "metres": 89,
      "yellow_cards": 0,
      "red_cards": 0
    }
  ]
}
```

---

## Weekly Admin Checklist (copy & paste each round)

```
□ Tuesday/Wednesday: Check for early team news & injury updates  
□ Thursday lunchtime: Team sheets announced — update via #admin  
□ Thursday evening / Saturday morning: Verify no late changes  
□ [LOCK TIME]: Confirm teams are locked (automatic)  
□ After final whistle: Collect results from sixnationsrugby.com  
□ After final whistle: Collect detailed stats from rugbypass.com  
□ Enter round JSON via #admin  
□ Verify league table updated correctly  
□ Post to group chat: scores are in, transfers open  
```

---

## Technical Details

- **Storage**: localStorage for team persistence across sessions
- **Data**: Fetches `round1.json`–`round5.json` on init (or loaded via Admin)
- **Admin**: Access via `#admin` hash — paste JSON to load data
- **Size**: ~41KB single HTML file
- **Mobile**: Responsive, works on 480px+ screens
- **No backend**: Everything runs client-side

---

## Deployment

1. Copy `index.html` to your GitHub Pages repo
2. Optionally pre-add `round1.json` through `round5.json` files
3. Access admin at `yoursite.github.io/#admin`
4. Share the link with your league: "The Armchair Coaches"

---

## Data Sources Reference

| Source | URL | Use For |
|--------|-----|---------|
| Six Nations Official | sixnationsrugby.com | Team sheets, match results, MoM |
| RugbyPass | rugbypass.com | Detailed player stats (Opta data) |
| BBC Sport | bbc.co.uk/sport/rugby-union | Team sheets, live text updates |
| National Unions | irishrugby.ie, ffr.fr, etc. | First to announce squads |
| PlanetRugby | planetrugby.com | Injury news between rounds |

---

## Future Enhancements (v2+)

- [ ] Firebase auth for multi-user leagues
- [ ] Countdown timer to transfer deadline
- [ ] AI-assisted team sheet parsing from social media posts
- [ ] Push notifications when teams are announced
- [ ] Historical stats and player form indicators

