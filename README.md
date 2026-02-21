# Z Extemp Timer (Offline App)

This build is a visual/functional copy of the timer and now works as an installable Progressive Web App (PWA), which can be installed on both Android (Chrome) and Windows (Edge/Chrome) and used offline.

## Run locally

```bash
python3 -m http.server 4173
```

Then open <http://localhost:4173>.

## Install on Android

1. Open the app URL in Chrome.
2. Tap the menu and choose **Add to Home screen**.
3. Launch from the home screen for standalone app mode.

## Install on Windows

1. Open the app URL in Edge or Chrome.
2. Choose **Install app** from the address bar/menu.
3. Launch it like a native app from Start Menu.

## Offline support

A service worker caches core app files (`index.html`, `logo.png`, and `manifest.webmanifest`) so the app can continue running without internet after first load.
