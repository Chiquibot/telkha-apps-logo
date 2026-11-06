# Telkha Apps — icons and home-screen launchers

Home-screen and browser-tab icons for the TAP ecosystem, plus a small launcher page per app so staff can add a proper icon to their phone.

| App | Launcher page | Icon |
|---|---|---|
| TAP | `/tap/` | `icons/tap-512.png` |
| TAP Pulse | `/pulse/` | `icons/pulse-512.png` |
| TAP Approval | `/approval/` | `icons/approval-512.png` |
| SAHOD | `/sahod/` | `icons/sahod-512.png` |
| TELKHA Cashflow | `/cashflow/` | `icons/cashflow-512.png` |

## Setup
1. **Settings → Pages →** Deploy from a branch → `main` / root. The site is then at `https://chiquibot.github.io/telkha-apps-logo/`.
2. Edit **`apps.js`** and paste each app's web-app URL (ends in `/exec`).
3. In each Apps Script project, set the Script property for the browser-tab icon:
   - TAP: `TAP_ICON_URL` = `https://chiquibot.github.io/telkha-apps-logo/icons/tap-512.png`
   - Pulse / Approval / SAHOD / Cashflow: `APP_ICON_URL` = the same address with `pulse-512.png`, `approval-512.png`, `sahod-512.png` or `cashflow-512.png`

## How staff install an icon
Send them the launcher link, e.g. `https://chiquibot.github.io/telkha-apps-logo/tap/`.
- **Android (Chrome):** tap *Install on this phone*.
- **iPhone (Safari):** Share → *Add to Home Screen*.

Tapping the icon afterwards opens the app directly. These pages hold no data; access to each app is still controlled by the app itself.

Each icon comes in 1024, 512, 192, 180 (iPhone) and 32 (browser tab) pixel sizes.
