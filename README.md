# Gym Plan PWA — Setup Instructions

## What's in this folder

```
index.html        — The app
manifest.json     — PWA metadata (name, icons, display mode)
sw.js             — Service worker (enables offline use)
icons/
  icon-192.png    — App icon (home screen)
  icon-512.png    — App icon (splash screen)
  favicon.ico     — Browser tab icon
README.md         — This file
```

---

## How to get this on your phone via GitHub Pages

### Step 1 — Create a GitHub account (if you don't have one)
Go to https://github.com and sign up. Free account is fine.

### Step 2 — Create a new repository
1. Click the **+** button (top right) → **New repository**
2. Name it: `gym-plan` (or anything you like)
3. Set it to **Public**
4. Click **Create repository**

### Step 3 — Upload the files
1. In your new repo, click **Add file** → **Upload files**
2. Drag the entire contents of this folder into the upload area:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - The `icons/` folder (all 3 files inside it)
3. Click **Commit changes**

### Step 4 — Enable GitHub Pages
1. Go to **Settings** (tab at the top of your repo)
2. In the left sidebar, click **Pages**
3. Under **Source**, select **Deploy from a branch**
4. Set branch to **main** and folder to **/ (root)**
5. Click **Save**
6. Wait 1–2 minutes. GitHub will show you a URL like:
   `https://yourusername.github.io/gym-plan`

### Step 5 — Install on your phone

**iPhone (Safari only — must use Safari, not Chrome):**
1. Open the URL from Step 4 in Safari
2. Tap the **Share** button (box with arrow pointing up)
3. Scroll down and tap **Add to Home Screen**
4. Tap **Add**
5. The app icon will appear on your home screen

**Android (Chrome):**
1. Open the URL in Chrome
2. Tap the three-dot menu
3. Tap **Add to Home Screen** or **Install App**
4. Tap **Install**

---

## Weight tracking

Weights you enter are saved to your phone's browser localStorage.
They persist as long as you:
- Always open the app from the home screen icon
- Don't clear your browser data

---

## Updating the app

If this plan is ever updated, just re-upload the new `index.html`
to your GitHub repo (drag and drop, same as before). The app on
your phone will update automatically next time you open it with
an internet connection.
