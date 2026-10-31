# BABA 777 — Free Hindi Casual Game

A mobile-first Hindi tap challenge with virtual coins, a daily free bonus, and a local leaderboard.

## Features
- Responsive Hindi UI for phones and desktop
- Tap to earn 1–5 virtual coins
- One free 50-coin daily bonus per browser date
- Save player name and local high scores
- No real-money deposits, betting, cash-out, or withdrawals
- Node.js built-in HTTP server; no third-party runtime packages required
- Health endpoint: `/health` and `/api/health`

## Run locally
Requires Node.js 18 or newer.

```bash
npm start
```

Open `http://localhost:10000`.

## Deploy on Render
1. Open Render and choose **New + → Web Service**.
2. Connect this repository: `ck160143-prog/Hindi-007`.
3. Runtime: **Node**.
4. Build command: leave empty (no build step is required).
5. Start command: `npm start`.
6. Deploy. Render provides the `PORT` environment variable automatically.
7. Open the service URL and check `/health` returns JSON with `"status":"ok"`.

If a Render service already points to this repository, check its service type and start command before changing settings. This repository's game is separate from the third-party website at hindi777agent1.com; pushing this code does not modify that external website.

## Important limitations
- Coins and leaderboard entries are stored in the current browser using localStorage. Clearing browser data can erase them.
- Scores are not synchronized across devices and are not protected against tampering. A real shared leaderboard needs a backend database and server-side validation.
- Coins are demo points only and have no cash value.
- Do not add real-money betting, deposits, withdrawals, or cash prizes without qualified legal review and all required permissions.

## Repository notes
The existing Hindi777 informational guides remain in this repository. The playable demo is served from `index.html`.

## License
MIT (see repository license terms).
