# W8out

Progressive web app: animated full body dumbbell workout guide. Yellow, black, zero dependencies, fully offline after first load.

## Structure

```
w8out/
  index.html        # the app
  manifest.json     # PWA manifest
  sw.js             # service worker, offline caching
  icons/
    icon.svg       # app icon
  README.md
```

## Deploy on GitHub Pages

1. Settings > Pages.
2. Source: Deploy from a branch. Branch: `main`, folder: `/ (root)`. Save.
3. Live at `https://vonbahr.github.io/w8out/` within a minute or two.

HTTPS is required for service workers, and GitHub Pages provides it, so offline caching and the install prompt work out of the box.

## Install as an app

- Android/Chrome: menu > Add to Home screen / Install app.
- iOS/Safari: Share > Add to Home Screen.
- Desktop/Chrome or Edge: install icon in the address bar, or the Install W8out button in the app.

## Icons

The manifest uses `icons/icon.svg`. For maximum Android compatibility you can add PNG icons (`icons/icon-192.png`, `icons/icon-512.png`) and reference them in `manifest.json`. Any square yellow dumbbell icon works if the filenames match the manifest.

## Features

- 8 animated dumbbell exercises: goblet squat, lunges, standing overhead press, bent over rows, hammer curls, floor press, Romanian deadlifts, overhead tricep extensions.
- Arrow buttons and dots to flip between exercises.
- Installable, offline-capable, zero build step, no frameworks.