# Tally Counter

A static, installable inventory tally counter. Organize items into folders and subfolders, tap +/- to count, edit names inline, and everything saves automatically to your device (browser localStorage) — no server, no account, works offline once installed.

## What it does

- **Folders & subfolders** — organize items into a tree (e.g. Warehouse → Shelf A → Screws)
- **Add / edit / delete** items and folders
- **Tally counting** — tap − / + or type a number directly, with a live tally-mark display
- **Search** across every item, from any folder
- **Export / Import** — download a JSON backup any time, and load it back in later or on another device
- **Installable PWA** — add it to your home screen / desktop from the browser, and it works fully offline afterward

All your data lives in the browser's local storage on your device. Nothing is sent anywhere. Use **Export** regularly if you want a backup file you control.

## Deploy it on GitHub Pages

1. Create a new GitHub repository (e.g. `tally-counter`).
2. Upload all the files in this folder (`index.html`, `manifest.json`, `sw.js`, and the `icons/` folder) to the root of that repository — keep the folder structure exactly as-is.
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to "Deploy from a branch," pick the `main` branch and `/ (root)` folder, then save.
5. Wait a minute or two, then GitHub will give you a URL like:
   `https://YOUR-USERNAME.github.io/tally-counter/`
6. Open that URL — the app should load.

## Installing it on your device

Once it's live on GitHub Pages:

- **Android (Chrome):** open the URL, tap the **⋮** menu → "Install app" (or you'll see an install banner automatically).
- **iPhone/iPad (Safari):** open the URL, tap the **Share** icon → "Add to Home Screen."
- **Desktop (Chrome/Edge):** open the URL, click the **install icon** (⊕ or a small monitor icon) in the address bar.

After installing, it opens like a normal app and works without an internet connection.

## Updating it later

If you edit any of the files and push the changes to GitHub, Pages will redeploy automatically. Because of the offline cache, people who already installed the app may need to fully close and reopen it once (or wait a moment) to pick up the update.

## Files in this folder

```
index.html       — the whole app (structure, style, and logic)
manifest.json    — PWA metadata (name, icons, colors) that makes it installable
sw.js            — service worker that caches the app for offline use
icons/           — app icons used for install/home-screen
```
