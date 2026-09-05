# Secret Word — Insider companion

A phone-friendly web app for running Insider-style party rounds: it secretly assigns
Master / Insider / Detective roles, shows the Master and Insider a single secret word,
and runs a round timer. English and Bulgarian included.

Two files, no build step:
- `index.html` — the app
- `words.json` — the word list (500 words, EN + BG paired)

## Deploy on GitHub Pages (2 minutes)

1. Create a new repo on GitHub (or use an existing one).
2. Upload **both** `index.html` and `words.json` to the root of the repo (they must sit
   next to each other — the app fetches `words.json` at startup).
3. Go to **Settings → Pages**, under "Build and deployment" set **Source** to
   `Deploy from a branch`, branch `main`, folder `/ (root)`, then **Save**.
4. Wait ~1 minute, then open the URL GitHub shows you (something like
   `https://yourusername.github.io/your-repo-name/`).

That's it — reopen that link on any phone to play. (If you ever test by just double-clicking
`index.html` on your computer instead of opening it through a server/Pages URL, the browser
may block the `words.json` fetch — the app falls back to a small 20-word built-in list in
that case so it still works, just with less variety.)

## How to play

1. **Set up round**: pick a player count (presets or a custom number for 9+), optionally
   type in player names, and toggle **Advanced Mode** if you want a 25% chance that no
   Insider exists that round at all.
2. **Start Game** assigns roles and picks one secret word.
3. Pass the phone around: each player taps their own name, then **holds** the reveal
   button. Detectives just see their role; the Master and Insider also see the secret
   word. Releasing the button hides it again immediately, and everyone can re-check their
   own role at any point during the round the same way — nothing is forced or automatic.
4. When the table's ready, start the timer (bottom bar: play/pause/reset) and begin
   asking yes/no questions to find the word before time runs out.

The ☰ menu (top right) has: language (English/Bulgarian), new round, and timer length
(quick presets or a custom number of minutes).
