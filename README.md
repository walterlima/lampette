# Lampette

A tiny web app that turns your iPhone into a mood light.

- Pick a color (presets or custom), intensity and how long it stays on (5 min to 2 hours, or no limit)
- The screen is kept awake while the light is on (Screen Wake Lock API, with a NoSleep.js video fallback for older iOS)
- When time is up, the light fades to black over 30 seconds and the phone is allowed to sleep again
- While the light is on: tap to see time left or stop, drag up/down to change intensity
- Settings are remembered between uses

## Put it on your iPhone

1. Merge into `main`, then in GitHub go to **Settings > Pages**, set **Source** to "Deploy from a branch", branch `main`, folder `/ (root)`, and save.
2. After a minute it is live at `https://<your-user>.github.io/lampette/`.
3. Open that URL in Safari, tap **Share > Add to Home Screen**. It now opens fullscreen like an app.

Tips: a web page cannot change the phone's real brightness, so set iPhone brightness where you like it and use the in-app intensity on top. Turn off Auto-Brightness and True Tone if the color drifts.

## Files

- `index.html` the whole app
- `NoSleep.min.js` keeps the screen on (v0.12.0, MIT, Rich Tibbett)
- `manifest.webmanifest`, `icon-*.png` home screen app metadata
