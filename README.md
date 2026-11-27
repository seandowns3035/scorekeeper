# Scorekeeper

A personal game-night scorekeeper: Skyjo, Flip 7: Vengeance, Five Crowns, Texas Chili, Skip-Bo, Phase 10, Farkle, and "Custom" for any other game (with teams). Includes a Timer tab and a Dice tab.

Plain static site — no build step. Everything lives in `index.html`.

## Deploy (Vercel)
1. Import this repo in Vercel. Framework preset: **Other**. No build command, no output directory.
2. Open the URL on your iPhone in Safari → Share → **Add to Home Screen**.

## Updating
1. Change `index.html`, bump `APP_VERSION` near the top of the script.
2. Bump `CACHE` in `sw.js` to match (e.g. `scorekeeper-v1.1`).
3. Commit and push. Vercel redeploys automatically.
4. Open the app, close it, open it again — the version at the bottom of the home screen confirms the update.

## Data
Players, favorites, the game in progress, and settings are stored on the device (localStorage). Nothing is sent anywhere.
