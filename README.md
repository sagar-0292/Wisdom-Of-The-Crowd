# Wisdom-Of-The-Crowd
## TripSplit — trip expense tracker (`trip-expense-tracker/`)

A mobile-first, installable web app (PWA) for tracking group trip expenses.

- Multiple trips, each with its own currency, optional budget and travellers
- Add expenses with category, payer, date, note, and an equal split among any subset of people
- Summary: total, per person, per day, spending by category / day / person, budget progress
- Settle up: minimal set of payments to square everyone up, with "Mark paid"
- Share summary (WhatsApp etc.), CSV export, JSON backup & restore
- Works offline, data stays on the device (localStorage), dark mode

**Run locally:** `cd trip-expense-tracker && python3 -m http.server 8000`, then open `http://<your-computer-ip>:8000` on your phone.
**Install on phone:** host the folder over HTTPS (e.g. GitHub Pages), open it, then "Add to Home Screen".
