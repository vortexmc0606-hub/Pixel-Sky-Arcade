# PixelSky Arcade

PixelSky Arcade is a browser-based collecting and mini-game project. It is a standalone fan-made game concept and is not affiliated with Blooket.

## Features

- Collectible buddy packs, rarity drops, duplicates, tickets, and the BuddyDex.
- Local player profile, achievements, daily bonus, and saved progress.
- Mini-games: Sky Quiz, Math Dash, Cloud Catch, Geo Jump, and Don't Look Down.
- A ticket-only Sky Flip room. Tickets have no cash value.
- Season 1 pass and first-visit navigation tour.
- Original SVG icons and buddy artwork, plus the embedded mascot PNG.
- Chat and Buddy Trading screens are currently placeholders; online accounts and multiplayer services are not implemented yet.

## Run Locally

Python 3 is sufficient to serve the static app:

```sh
python3 -m http.server 8000 --bind 0.0.0.0
```

Open <http://localhost:8000> in a browser. The game is implemented in `index.html`; the custom Brain Rot pack artwork is in `assets/brain-rot-pack.svg`.

## Save Data

Player progress is stored in the browser's local storage. It does not sync between browsers or devices. Use **Settings → Reset All Progress** to clear the local save.

## Backend Roadmap

The current build has no server. Registration, login, online chat, and buddy trading will need a backend with persistent accounts, authenticated sessions, and server-validated inventory and trade transactions before they can work across devices.
