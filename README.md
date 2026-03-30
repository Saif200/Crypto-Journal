# CryptoJournal 📊

A personal crypto trading journal with PIN-based login, installable as a mobile app (PWA).

## Files

| File | Purpose |
|------|---------|
| `index.html` | Main app (login + journal) |
| `manifest.json` | PWA manifest for "Add to Home Screen" |
| `sw.js` | Service worker for offline support |
| `icon-192.png` | App icon (Android/PWA) |
| `icon-512.png` | App icon (splash screen) |

## Deploy to GitHub Pages

1. Create a new **public** GitHub repository (e.g. `crypto-journal`)
2. Upload all 5 files to the repository root
3. Go to **Settings → Pages**
4. Under *Source*, select **Deploy from a branch**
5. Choose `main` branch, `/ (root)` folder → click **Save**
6. Your app will be live at: `https://YOUR_USERNAME.github.io/crypto-journal/`

## First-Time Setup

1. Open your GitHub Pages URL
2. You'll be prompted to **set a 4-digit PIN** — this secures your journal
3. Set your starting capital
4. Start logging trades!

## Install on Mobile

### Android (Chrome)
- Open the app URL in Chrome
- Tap the **Install** banner at the bottom, or
- Tap the **⋮ menu → Add to Home Screen**

### iPhone (Safari)
- Open the app URL in Safari
- Tap the **Share button (□↑)**
- Tap **Add to Home Screen**

## Security Notes

- The PIN is hashed with SHA-256 (10,000 iterations) before storage
- All data stays **local to your device** — nothing is sent to any server
- Use the **🔒 Lock** button to lock the app when done
- Change your PIN anytime via the **⚙ PIN** button in the header

## Privacy

All trade data is stored in your browser's `localStorage`. No accounts, no servers, no cloud.
