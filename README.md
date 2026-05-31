# Gym Plan PWA — Setup & Reference Guide

A Progressive Web App (PWA) version of your 5-day stunt performer training plan.
Once installed, it works like a native app — offline, full screen, with persistent weight tracking.

---

## What's in the zip

```
gym_pwa/
├── index.html        The app itself
├── manifest.json     PWA config (name, icons, display mode)
├── sw.js             Service worker — enables offline use
├── icons/
│   ├── icon-192.png  Home screen icon
│   ├── icon-512.png  Splash screen icon
│   └── favicon.ico   Browser tab icon
└── README.md         This file
```

---

## First-time setup — GitHub Pages

### 1. Create a GitHub account
Go to **https://github.com** and sign up. A free account is all you need.

### 2. Create a new repository
- Click the **+** button (top right) → **New repository**
- Name it something like `gym-plan`
- Set visibility to **Public**
- Click **Create repository**

### 3. Upload the files
- In your new repo, click **Add file** → **Upload files**
- Unzip the downloaded file and drag the entire contents of the `gym_pwa/` folder into the upload area:
  - `index.html`
  - `manifest.json`
  - `sw.js`
  - The `icons/` folder with all 3 files inside
- Add a commit message (e.g. "Initial upload") and click **Commit changes**

### 4. Enable GitHub Pages
- Go to **Settings** (tab along the top of your repo)
- In the left sidebar, click **Pages**
- Under **Source**, select **Deploy from a branch**
- Set branch to **main**, folder to **/ (root)**
- Click **Save**
- Wait 1–2 minutes. Your app URL will appear at the top of the Pages screen:

```
https://yourusername.github.io/gym-plan
```

---

## Installing on your phone

### iPhone — must use Safari
1. Open your GitHub Pages URL in **Safari** (not Chrome)
2. Tap the **Share** button — the box with an arrow pointing up, at the bottom of the screen
3. Scroll down in the share sheet and tap **Add to Home Screen**
4. Give it a name (or leave as default) and tap **Add**
5. The app icon will appear on your home screen

> **Important:** Always open the app from the home screen icon, not from Safari directly.
> This keeps it in standalone mode and ensures your saved weights persist correctly.

### Android — Chrome
1. Open your GitHub Pages URL in **Chrome**
2. Tap the three-dot menu (top right)
3. Tap **Add to Home Screen** or **Install App**
4. Tap **Install**
5. The app icon will appear on your home screen

---

## Using the app

| Feature | How it works |
|---|---|
| **Day selection** | Tabs at the top — D1 through D5. Blue dot = swim day. |
| **Exercises** | Tap any exercise row to expand it and see coaching notes. |
| **Weight tracking** | Four week input fields per exercise. Type and move on — saves automatically. |
| **Exercise guide** | Tap 📖 on any expanded exercise for full setup, steps, and coaching points. |
| **Rest timer** | Tap ⏱ to start a countdown. Defaults to 90s. Tap 60s to switch. Vibrates on completion. |
| **Pull-up tracker** | Visible on Day 2 — shows your current stage and what comes next. |

---

## Weight tracking — persistence

Weights are saved to your phone's browser **localStorage**, tied to how the app is opened.

**Weights will persist if you:**
- Always open the app from the **home screen icon**
- Use the same phone

**Weights will be lost if you:**
- Clear your browser's site data or cache
- Open the app from a different browser or device

There is no cloud sync — weights live on the device only.

---

## Updating the app

If the plan is ever revised and you receive a new `index.html`:

1. Go to your GitHub repo
2. Click on `index.html` in the file list
3. Click the **pencil** (edit) icon, or use **Add file → Upload files** to replace it
4. Commit the change

The app on your phone will update automatically the next time you open it with an internet connection. Your saved weights are unaffected by updates.

---

## Troubleshooting

| Problem | Fix |
|---|---|
| "Add to Home Screen" not showing on iPhone | Make sure you're using Safari, not Chrome or another browser |
| App not updating after a file change | Close and reopen the app, or clear the app's cache in phone settings |
| Weights disappeared | Check you opened via the home screen icon, not the browser. Also check browser data hasn't been cleared. |
| GitHub Pages URL not working | Wait a few minutes after enabling Pages — it can take up to 5 minutes to go live |
| App shows old version | On iPhone: hold the home screen icon → Remove App → reinstall from Safari |

---

## Your GitHub Pages URL

Once set up, note your URL here:

```
https://_________________________________.github.io/gym-plan
```

---

*Built for your 5-day stunt performer training plan. Cluster format, eccentric focus, pull-up progression.*
