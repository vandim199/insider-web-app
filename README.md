# Secret Word — Insider companion

A single-file phone-friendly web app for running the word-reveal part of an Insider-style
party round: 5 random words, a secret one only the Master and Insider get to see, and a
round timer. No build step, no dependencies — just one HTML file.

## Deploy on GitHub Pages (2 minutes)

1. Create a new repo on GitHub (or use an existing one).
2. Upload `index.html` to the root of the repo (drag-and-drop on the GitHub web UI works).
3. Go to **Settings → Pages**, under "Build and deployment" set **Source** to
   `Deploy from a branch`, branch `main`, folder `/ (root)`, then **Save**.
4. Wait ~1 minute, then open the URL GitHub shows you (something like
   `https://yourusername.github.io/your-repo-name/`).

That's it — reopen that link on any phone to play.

## How to run it

- **Start new round** picks 5 random words and starts the private reveal.
- Pass the phone to the **Master** first, then the **Insider** — each holds the
  reveal button to privately see which word is correct, then taps continue.
- The word list (without the highlight) stays on screen for everyone during the round,
  along with a 5-minute timer at the bottom (play/pause/reset).
- The ☰ menu (top right) lets you view the secret again mid-round, start a new round,
  or change the timer length.
