# Job Application Tracker

A clean, fast, single-file job application tracker that runs entirely in the browser — no backend, no signup, no dependencies.

Built for engineers who want to stay organised during a job search without the overhead of a full SaaS tool.

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Single file](https://img.shields.io/badge/size-single%20HTML%20file-blue)
![No dependencies](https://img.shields.io/badge/dependencies-none-green)

---

## Features

- **Track every application** — company, role, status, priority, date, salary range, referral contact, hiring manager, interview rounds, next action, and notes
- **Pipeline view** — filter by Wishlist / Applied / Screening / Interview / Offer / Rejected
- **Live stats** — total tracked, in pipeline, offers received, interview conversion rate
- **Detail side panel** — click any row to see full application details
- **Search** — filter by company or role in real time
- **Export CSV** — download all your data at any time
- **Dark mode** — auto-detects system preference
- **Keyboard shortcuts** — `N` to add, `Esc` to close modals
- **Persists locally** — data saved in `localStorage`, survives page refresh
- **Zero dependencies** — one HTML file, no npm, no build step, no internet required

---

## Quick start

```bash
# Option 1: Open directly in browser
open index.html

# Option 2: Serve locally (optional)
python3 -m http.server 8080
# then open http://localhost:8080
```

That's it. No installation. No build step.

---

## Usage

| Action | How |
|--------|-----|
| Add application | Click **+ Add application** or press `N` |
| View details | Click any table row |
| Edit | Hover a row → click the edit icon, or open detail panel → Edit |
| Delete | Hover a row → click the delete icon |
| Filter by status | Click the status pills in the toolbar |
| Search | Type in the search box (filters company + role) |
| Export | Click **↓ Export CSV** (top right) |
| Clear all | Click **Clear all data** (bottom right) |

---

## Status meanings

| Status | Meaning |
|--------|---------|
| Wishlist | Companies you want to apply to |
| Applied | Application submitted, waiting for response |
| Screening | Recruiter screen or initial HR call |
| Interview | Active interview rounds in progress |
| Offer | Offer received |
| Rejected | Application declined at any stage |
| Withdrawn | You withdrew your application |

---

## Data & privacy

All data is stored in your browser's `localStorage`. Nothing is sent to any server. Clearing your browser data will erase tracker data — use **Export CSV** regularly to back up.

---

## Customising

The entire app is one HTML file with no external dependencies. Edit it directly:

- **Add a new status** — update the `<select id="f-status">` options and the `STATUS_CLASS` object in the script
- **Add a new field** — add an input in the form grid, add the field name to the `FIELDS` array, and add it to the detail panel render
- **Change colours** — edit the CSS custom properties in `:root`

---

## Contributing

PRs welcome. Keep it dependency-free and single-file.

---

## Author

Built by [Parikshit Sharma](https://linkedin.com/in/parikshitlitb) — Senior AI/ML Engineering Leader

---

## License

MIT
