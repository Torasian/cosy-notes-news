# Cosy Notes news

`feed.json` is read by the Cosy Notes app at launch to show announcements
and the early bird offer without an App Store update. It is served by
GitHub Pages at https://torasian.github.io/cosy-notes-news/feed.json.

- Each announcement shows once per device; give a new announcement a new `id`.
- `audience`: `everyone`, `free` or `unlocked`. Dates are `yyyy-MM-dd`.
- A button has `url` (https only) or `"action": "unlock"`.
- `earlyBird.newPrices` is keyed by App Store country (ISO alpha-3) and
  must match the prices scheduled in App Store Connect.
- Keep it valid JSON: an invalid file is ignored and the app keeps the last good copy.
