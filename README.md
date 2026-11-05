# Bills Must Be Paid — Free Browser Game 🐷🔨

An original, free browser game inspired by the piggy-smashing incremental genre
(the linked Google Play title *Bills Must Be Paid* by Rike Games costs $5.99).
This version is written from scratch — its own code, no copied assets — and
runs 100% in the browser. No download, no sign-up, no server.

## Play it
Open `index.html` in any browser, or host it (below) and share the link.

## Host on GitHub Pages (free, ~3 minutes)
1. Create a new **public** GitHub repo named `bills-must-be-paid-web`
   (github.com → New repository).
2. Upload these files to the repo root: `index.html`, `README.md`,
   `robots.txt`, `sitemap.xml` (drag-and-drop on the repo page →
   "uploading an existing file" → Commit).
3. In the repo: **Settings → Pages → Build and deployment → Source:
   Deploy from a branch → Branch: `main` / `(root)` → Save.**
4. Wait ~1 minute. Your game is live at:
   **https://ankitgarg43.github.io/bills-must-be-paid-web/**
5. If you name the repo something else, update the `<link rel="canonical">`
   URL and `sitemap.xml` to match, so search engines index it correctly.

## How to play
- **Click / tap piggy banks** to smash them for coins. Every swing costs stamina — when your hand gives up, rest (stress +10%) or declare bankruptcy.
- **Pay bills** before their timers run out. Overdue bills charge interest and raise Stress; Stress at 100% forces bankruptcy. Paying a bill = a free perk (pick 1 of 3) + Legacy Points.
- **7 piggy types:** Classic, Baby, Runner (fast!), Lazy (tanky), Armoured, Black-Money (rich + sneaky), and the rare GOLDEN piggy.
- **Skill tree (7 upgrades):** Grip Strength, Wrist Pump, Hit the Gym, Caffeine Addiction, Get Lucky, Rock Rain ability, Electrify ability.
- **6 hammers** with real trade-offs: damage / speed / splash radius / crit.
- **Abilities:** Rock Rain, Electrify, Coffee Rush — plus surprise Piggy Rain and Coin Frenzy events.
- **Rare coins:** 8 collectibles hidden in piggies.
- **Bankruptcy = prestige:** reset the run, keep Legacy Points, and buy permanent Rings, Bracelets and Lucky Charms.
- **Win:** pay 15 bills to become Debt-Free, then endless mode.
- Progress **auto-saves** in the player's browser (localStorage). Sound and music are generated in-browser (Web Audio) — no audio files needed.

## Tech
Single self-contained `index.html` (HTML + CSS + vanilla JS, canvas-rendered
arena with hand-drawn piggies, crack/shatter/particle effects). Works on
desktop and mobile. No build step, no dependencies.

## Version 2 (Nov 5, 2026)
Rebuilt after v1 play-test feedback ("it's bad"): canvas engine instead of
emoji pigs, progressive cracking, screen shake, ceramic-shard and coin
particles, rebalanced economy (cheaper first bill, 1-stamina swings, faster
regen), and a fixed bill panel that no longer re-renders every frame.
To update an existing GitHub Pages deployment, just replace `index.html`
in the repo — Pages redeploys automatically in about a minute.
