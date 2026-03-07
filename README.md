# Z Extemp Timer (Offline App)

This build is a visual/functional copy of the timer and works as an installable Progressive Web App (PWA), which can be installed on both Android (Chrome) and Windows (Edge/Chrome) and used offline.

## What changed

- The live clock now shows **hours, minutes, and seconds**.
- The service worker cache version was bumped so installed apps can receive this update.
- Added an in-app **Install App** button for browsers that support install prompts.

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

## Install on iPhone/iPad

1. Open the app URL in **Safari**.
2. Tap **Share**.
3. Tap **Add to Home Screen**.
4. Tap **Add**.

## Offline support

A service worker caches core app files (`index.html`, `logo.png`, and `manifest.webmanifest`) so the app can continue running without internet after first load.

## If an installed app does not update immediately

1. Open the app while connected to internet.
2. Close it, then reopen it.
3. If still stale, refresh the page in browser once and reinstall/open again.

## If you must press Ctrl+F5 to see updates

1. Open the app URL once while online and wait a few seconds.
2. Close all tabs/windows for the app and reopen it.
3. If still stale, uninstall/reinstall the installed app shortcut once.

## If you do not see an install option

- **Windows (Edge/Chrome):** look for **Install App** in the address bar or app menu.
- **Android (Chrome):** menu → **Add to Home screen**.
- **iPhone/iPad (Safari):** Share → **Add to Home Screen** (Apple does not use the same install prompt button).
