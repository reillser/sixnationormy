# Fantasy Rugby Six Nations 2026 — "The Armchair Coaches"

A single-page Fantasy Rugby web app for the 2026 Six Nations Championship.  
Built as one `index.html` file (~51KB) for GitHub Pages. No external dependencies — pure HTML/CSS/JS.

---

## Quick Start

1. Copy `index.html` to your GitHub Pages repository
2. Push to deploy
3. Share the URL with your league members
4. Admin manages data via `yoursite.github.io/#admin`

---

# 📖 User Guide — How to Play

## The Basics

You are the manager of a fantasy rugby team. Pick 15 real Six Nations players, earn points based on how they perform in actual matches, and compete against other managers in your league.

**Your goal:** Score the most points across all 5 rounds of the Six Nations to win "The Armchair Coaches" league.

---

## Building Your Squad

### Budget & Limits
- **€100m budget** — spend it wisely across 15 players
- **15 players total**: 11 starters + 4 on the bench
- **Max 5 players per nation** — you can't just stack all Irish players!
- **Player prices range from €5m to €12m** — elite players cost more but score more

### Positions (11 starters)
Your starting XV must include:

| Position | Count | Role |
|----------|-------|------|
| **Full Back** | 1 | Last line of defence, counter-attacks |
| **Wing** | 2 | Try scorers, finishers |
| **Centre** | 2 | Midfield runners, defenders |
| **Fly Half** | 1 | Playmaker, kicker (big points potential) |
| **Scrum Half** | 1 | Links forwards and backs |
| **Number 8** | 1 | Ball carrier, link player |
| **Flanker** | 2 | Tacklers, turnovers, breakdown workers |
| **Lock** | 2 | Lineout, carries, tackling machines |
| **Prop** | 2 | Scrummaging, carrying (cheap squad fillers) |
| **Hooker** | 1 | Lineout thrower, tackler |

### Bench (4 players)
- Bench players earn **half points** — they're your insurance
- Pick a mix of forwards and backs for flexibility
- Good bench picks: cheap players in key positions, or a premium player you can't afford to start

---

## Scoring System — How Points Are Earned

### Attack (the big earners)

| Action | Points | Notes |
|--------|--------|-------|
| **Try** | +20 | The biggest single action. Back-row and wings score most |
| **Try Assist** | +10 | The final pass before a try |
| **Conversion** | +3 | After each try — fly halves and full backs |
| **Penalty Goal** | +3 | Steady points for accurate kickers |
| **Drop Goal** | +10 | Rare but valuable |
| **Clean Break** | +5 | Breaking through the defensive line |
| **Offload** | +3 | Passing in the tackle — skilful backs |
| **Metres Made** | +0.1 per metre | Adds up! A winger making 80m = 8pts |
| **Defenders Beaten** | +1 | Evading tackles |

### Defence (the grinders)

| Action | Points | Notes |
|--------|--------|-------|
| **Tackle Made** | +1 | Flankers/locks can make 15+ per game = 15pts |
| **Turnover Won** | +7 | Jackaling at the breakdown — flanker territory |
| **Lineout Steal** | +5 | Disrupting opposition ball — tall locks |

### Bonuses

| Action | Points | Notes |
|--------|--------|-------|
| **Winning Team** | +5 | All 23 players on a winning team get this |
| **Man of the Match** | +15 | One per match — big swing |
| **Hat-trick Bonus** | +10 | Extra reward for 3+ tries |

### Penalties (negative points)

| Action | Points | Notes |
|--------|--------|-------|
| **Missed Tackle** | -1 | Poor defenders get punished |
| **Penalty Conceded** | -3 | Ill-disciplined players cost you |
| **Yellow Card** | -10 | 10 minutes off and -10 pts |
| **Red Card** | -20 | Game over and a massive point hit |

### Captain & Bench Multipliers

| Rule | Effect |
|------|--------|
| **Captain** | Scores **×1.5** — choose your captain carefully each round |
| **Bench players** | Score **half points** — starters are always more valuable |

---

## Strategy Tips

### Captain Selection
- Pick a player likely to have a **big game** — not just a safe pick
- Fly halves in matches against weaker teams (kicking points + try involvements)
- Back-row forwards in tight matches (tackle counts rack up)
- Louis Bielle-Biarrey was the tournament's top scorer — wingers CAN be great captains

### Budget Strategy
- **Don't blow it all on stars** — you need 15 players within €100m
- A €12m player needs to outscore two €6m players combined to be worth it
- **Props are cheap (€5-7m)** and can still score well through tackles
- **Fly halves are value** — they kick conversions AND penalties (+3 each time)

### Transfer Tactics
- **2 free transfers per round** — use them wisely
- Extra transfers cost **-5 points each** — only do it if the gain is clear
- Watch for injuries announced on Thursday — swap injured players out!
- Target players facing weak opposition (check the fixture)

### Bench Decisions
- Bench players earn half points — it's always better to START your best
- Use the bench for: injury cover, cheap nation-slot fillers, and fixture rotation
- If unsure between two similar players, start the one with the easier fixture

### Fixture Awareness
- Teams playing at HOME tend to score more
- Look at the previous round's results for form indicators
- **France at home** were devastating in 2026 (36-14, 54-12, 48-46!)
- **Italy at home** pulled off upsets (beat England 23-18 in Round 4)

---

## Transfers & Deadlines

### How Transfers Work
- You get **2 free transfers between each round**
- Want more? Each extra transfer costs **-5 points** from your total
- Changes must be made **before the deadline** (first kickoff of the round)

### Deadline Lock
- All teams lock at the **first kickoff of the round**
- After lock, you CANNOT change your team, captain, or bench order
- The countdown timer on the app shows how long you have left
- **Set a reminder!** Thursday evening or Saturday morning depending on the round

---

## The League

### How It Works
- Everyone in the league picks their own team independently
- Points accumulate across all 5 rounds
- Final standings after Round 5 determine the winner
- Head-to-Head comparisons available in the H2H tab

### Viewing Your Score
- **My Team tab**: See your current round score and pitch layout
- **League tab**: See the full standings table with all 5 round columns
- **H2H tab**: Compare yourself directly against any other manager
- **Results tab**: See match results and top scorers for each round

---

## 2026 Six Nations Player Database

The app includes **211 players** who featured across all 5 rounds:
- **France**: 35 players (Champions 🏆)
- **Ireland**: 38 players
- **England**: 37 players
- **Scotland**: 36 players
- **Wales**: 35 players
- **Italy**: 30 players

### Key Players to Know

| Player | Nation | Position | Price | Why Pick Them |
|--------|--------|----------|-------|---------------|
| Antoine Dupont | France | Scrum Half | €12.0m | Best player in the world, try assists machine |
| Louis Bielle-Biarrey | France | Wing | €11.0m | 8 tries in 2026 — Player of the Tournament |
| Caelan Doris | Ireland | Number 8 | €11.0m | Captain, carries and tackles galore |
| Finn Russell | Scotland | Fly Half | €10.5m | Unpredictable genius, kicking points |
| Maro Itoje | England | Lock | €10.0m | Tackle machine, lineout steals |
| Paolo Garbisi | Italy | Fly Half | €9.0m | Italy's kicker — steady penalty points |

---

## Tips for New Players

1. **Don't overthink Round 1** — just pick players you like and learn the scoring
2. **Check the app on Thursday** — that's when team sheets come out
3. **Set your captain before the deadline** — forgetting costs you 50% of their bonus!
4. **Watch for yellow cards** — a player on -10 can ruin your week
5. **Have fun** — it's called "The Armchair Coaches" for a reason 🍺

---
---

# ⚙️ Admin Guide — Running the League

You (the league admin) manage the data each round. Here's your workflow:

## Admin Instructions — Round-by-Round Workflow

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

> ⚡ **Tip:** Check again on match morning — late changes occasionally happen after the captain's run.

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
2. Once locked, managers cannot make transfers or change their captain
3. Remind the league: _"Teams lock at [TIME] — get your transfers in!"_

### 📊 Step 3: Enter Match Results & Scoring (after all games complete)

**When:** After the final whistle of the last match in the round.

**Where to get scoring data:**
1. **Match results & try scorers**: [sixnationsrugby.com](https://www.sixnationsrugby.com) → Match Centre
2. **Detailed stats** (tackles, carries, offloads, metres): [rugbypass.com](https://www.rugbypass.com) → Match Stats (Opta-powered)
3. **Man of the Match**: Usually announced on broadcast / sixnationsrugby.com
4. **Kicking stats** (conversions, penalties): Match Centre on sixnationsrugby.com

**What to do:**
1. Go to `yoursite.github.io/#admin`
2. Create the **round results JSON** (see format below)
3. For each match, record: final score, try scorers, conversions/penalties, cards, MoM, detailed stats
4. Paste the JSON into Admin panel and click **Load Data**
5. The scoring engine automatically calculates points for all players
6. Check the League Table updates correctly

> ⚡ **Tip:** Start with tries + kicking + cards + MoM (the big point-scorers). Add detailed stats later.

### 🔄 Step 4: Open Next Round for Transfers

**When:** After scoring is loaded and verified.

**What to do:**
1. Update the player database with any new squad members (injury replacements)
2. Set the next round's deadline
3. Post to the group: _"Round X scores are in! Transfers open for Round Y."_

---

## Round Data JSON Formats

### Team Sheets (pre-round)

```json
{
  "round": 1,
  "deadline": "2026-02-05T20:10:00Z",
  "team_sheets": [
    {
      "team": "France",
      "starting_xv": [
        {"number": 1, "name": "Jean-Baptiste Gros", "position": "Prop"},
        {"number": 9, "name": "Antoine Dupont", "position": "Scrum Half"}
      ],
      "replacements": [
        {"number": 16, "name": "Peato Mauvaka", "position": "Hooker"}
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
  "players": [
    {
      "id": 2,
      "stats": {
        "try": 2,
        "clean_break": 3,
        "metres": 89,
        "defenders_beaten": 4,
        "tackle": 4,
        "winning_team": true
      }
    }
  ]
}
```

---

## Weekly Admin Checklist

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
- **Size**: ~51KB single HTML file
- **Mobile**: Responsive, works on 480px+ screens
- **No backend**: Everything runs client-side
- **Players**: 211 across all 6 nations (full tournament squads)

---

## Deployment

1. Copy `index.html` to your GitHub Pages repo
2. Optionally pre-add `round1.json` through `round5.json` files
3. Access admin at `yoursite.github.io/#admin`
4. Share the link with your league: "The Armchair Coaches"

For GitHub Actions, add this to your workflow to avoid the Node.js 20 deprecation warning:
```yaml
env:
  FORCE_JAVASCRIPT_ACTIONS_TO_NODE24: true
```

Or simpler: go to Settings → Pages → deploy from branch (no workflow needed).

---

## Data Sources Reference

| Source | URL | Use For |
|--------|-----|---------|
| Six Nations Official | sixnationsrugby.com | Team sheets, match results, MoM |
| RugbyPass | rugbypass.com | Detailed player stats (Opta data) |
| BBC Sport | bbc.co.uk/sport/rugby-union | Team sheets, live text updates |
| National Unions | irishrugby.ie, ffr.fr, etc. | First to announce squads |
| PlanetRugby | planetrugby.com | Injury news between rounds |
