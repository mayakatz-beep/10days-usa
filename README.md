# 🗺️ 10 Days in the USA

A browser-based multiplayer board game based on **10 Days in the USA** — play with friends online or against AI bots, all in a single HTML file with no server required.

🎮 **[Play Live →](https://mayakatz-beep.github.io/10days-usa/)**

---

## Features

- **Multiplayer P2P** — create a room, share a 4-letter code, play with up to 4 people with no account or server needed (powered by PeerJS)
- **AI Bots** — play offline against 1–3 bots with a greedy-search AI
- **Interactive USA map** — color-coded states, click-to-pin any state to highlight its neighbors and borders
- **Northeast panel** — VT, NH, MA, RI, CT, NJ, DE, MD displayed in a readable side panel with leader lines
- **Full game rules enforcement** — adjacency, car (two-hop), airplane (same color), Alaska/Hawaii wildcards
- **Session persistence** — game saves to localStorage; resume after accidental page close
- **Mobile-friendly** — 44px touch targets, swipe-down to close map, responsive layout

---

## How to Play

| Connection | Rule |
|-----------|------|
| 🚶 On foot | Two **adjacent** (bordering) states sit next to each other directly |
| 🚗 Car | Place between two states with **one state between** them |
| ✈️ Airplane | Place between two states of the **same color** (Alaska & Hawaii are wildcards) |

1. Each player places 10 tiles one-by-one into their journey slots (days 1–10)
2. On your turn: draw from the deck or a discard pile, then swap a tile in your journey or discard it
3. When your 10-day route is valid end-to-end, hit **🔍 Check** then **🎉 Declare!** to win

---

## Tech Stack

- **Vanilla HTML/CSS/JS** — zero build tools, zero dependencies installed
- **[PeerJS](https://peerjs.com/)** — WebRTC P2P networking
- **[D3.js](https://d3js.org/) + [TopoJSON](https://github.com/topojson/topojson)** — SVG map rendering
- **Google Fonts** — Bebas Neue + DM Sans

---

## Run Locally

Just open `index.html` in any modern browser — no server or install needed.

```bash
git clone https://github.com/mayakatz-beep/10days-usa.git
cd 10days-usa
open index.html   # macOS
# or double-click index.html on Windows
```

---

*Based on the board game [10 Days in the USA](https://boardgamegeek.com/boardgame/1376/10-days-in-the-usa) by Alan R. Moon & Aaron Weissblum.*
