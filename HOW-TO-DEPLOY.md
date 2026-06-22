# Courage Loop — getting it on your phone (free, no app store)

This is a PWA: a web app that installs as an icon and runs fully offline.
All your data stays on your phone. Nothing is sent anywhere. No account, no payment.

You'll host it free on **GitHub Pages** — you already have a GitHub account.

---

## Part 1 — Put the files on GitHub (10 min, do this on a computer)

1. Go to https://github.com/new
2. Repository name: `courage-loop`
3. Set it to **Public** (Pages needs this on the free plan). Public only means the *code* is visible — **your saved events are NOT in the code**, they live only on your phone. Nobody can see your data.
4. Tick **"Add a README file"**, then click **Create repository**.
5. On the repo page, click **Add file → Upload files**.
6. Drag in ALL of these files:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
   - `icon-180.png`
   - `icon-maskable-512.png`
7. Click **Commit changes**.

## Part 2 — Turn on GitHub Pages (2 min)

1. In the repo, go to **Settings** (top menu) → **Pages** (left sidebar).
2. Under "Build and deployment", Source = **Deploy from a branch**.
3. Branch = **main**, folder = **/ (root)**. Click **Save**.
4. Wait ~1 minute, refresh the page. You'll see a green link like:
   `https://YOURNAME.github.io/courage-loop/`
5. Open that link. The app should load.

## Part 3 — Install it on your phone (1 min)

Open that same link **on your phone's browser**, then:

**iPhone (Safari):**
- Tap the **Share** button (square with up-arrow)
- Scroll down → **Add to Home Screen** → **Add**

**Android (Chrome):**
- Tap the **⋮** menu (top right)
- **Add to Home screen** / **Install app** → **Install**

Now there's a Courage Loop icon on your home screen. It opens full-screen with no
browser bars, and works with no internet.

---

## Looking after your data

Your events live in your phone's browser storage. That means:
- **Private** — never leaves the device.
- **Fragile** — if you clear your browser data or switch phones, it's gone.

So: every few weeks, open the app → tap the **gear icon** → **Export backup**.
That saves a small file you can email to yourself. If you ever need it back,
gear icon → **Restore from backup**.

---

## Changing things later

Everything is in `index.html`. The lists you'll most likely want to edit are near
the top of the `<script>` section:
- `EVENT_TYPES` — the events you can prepare for
- `PREDICTIONS` — the fears you can tap (you can also add your own in-app)
- `EVIDENCE` — the evidence options on review
- `BIASES` — the thinking-bias checklist

Edit the file, re-upload it to GitHub (same Upload files step, it overwrites),
and the live app updates within a minute. On your phone you may need to close and
reopen it once to pull the new version.
