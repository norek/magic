# 🃏 MTG Commander Stats Dashboard

Interactive statistics dashboard for our Magic: The Gathering Commander group.

**Live:** [norek.github.io/magic](https://norek.github.io/magic/)

## Features

- **📊 Overview** — player rankings, win rates over time, first player advantage, 3v4 player analysis
- **👤 Players** — per-player deep dive with deck WR, session history, cumulative performance
- **🃏 Decks** — per-deck view showing who plays it, progression over time, streaks
- **🆚 Head-to-Head** — matchup matrix, rivalry visualizations
- **🎨 Colors** — MTG color identity analysis (data from Scryfall API), color combinations WR, radar profiles
- **💪 Power Rating** — Wilson Score + Bayesian ranking that accounts for sample size
- **💰 CMC Analysis** — commander mana cost vs performance correlation
- **⚔️ Matchups** — dynamic deck-vs-deck counter-pick guide (any player vs any player)
- **⭐ Fun Facts** — records, awards, trivia

## Data

Games are tracked in `MTG Games - Games.csv`. Format:

```
Date,Winner,First Player,P1,P1 Deck,P2,P2 Deck,P3,P3 Deck,P4,P4 Deck
```

## Tech

Single-file HTML dashboard. No build step, no dependencies to install.

- Chart.js 4.4 (CDN)
- Vanilla JS
- Commander color identities & CMC from [Scryfall API](https://scryfall.com/docs/api)

## Stats

- 91 games across 27 sessions (Jan 2024 – Jun 2026)
- 6 players, 62 unique decks
- ~80KB total page size
