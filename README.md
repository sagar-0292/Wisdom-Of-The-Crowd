# Wisdom-Of-The-Crowd
## TripSplit — trip expense tracker (`trip-expense-tracker/`)

A mobile-first, installable web app (PWA) for tracking group trip expenses.

- Multiple trips, each with its own currency, optional budget and travellers
- Add expenses with category, payer, date, note, and an equal split among any subset of people
- Summary: total, per person, per day, spending by category / day / person, budget progress
- Settle up: minimal set of payments to square everyone up, with "Mark paid"
- **Share trips with your group** — one link carries the whole trip (no accounts, no server). Friends open it to get a copy;
  when they add expenses they tap *Sync trip* and send their link back, and opening it merges the changes
  (new and edited expenses are combined, deletions carry over, opening the same link twice is harmless)
- Share a text summary (WhatsApp etc.), invite friends to the app, CSV export, JSON backup & restore
- Works offline, data stays on the device (localStorage), dark mode

**Run locally:** `cd trip-expense-tracker && python3 -m http.server 8000`, then open `http://<your-computer-ip>:8000` on your phone.
**Publish it (one-time):** in the GitHub repo go to *Settings → Pages → Build and deployment → Source* and pick **GitHub Actions**.
Every push to `main` that touches `trip-expense-tracker/` then deploys it to
`https://sagar-0292.github.io/Wisdom-Of-The-Crowd/`. Open that on your phone and choose "Add to Home Screen".
