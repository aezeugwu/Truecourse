# TrueCourse v0.1.0

Personal Cycle & Execution OS — the merged successor to PC-EOS and 60D-POS.

## What's in this build

- Home: live Day Score / Execution Ratio / Alignment Score, Today's Execution
  timetable, Practice snapshot, This Cycle's Vision (WOOP), Accountability
  share card, Tomorrow preview
- Practice: Morning / Afternoon / Evening sub-tabs
- Log: Block Activity (project, actual time, progress, 12-pair Intent/Actual
  tagging) and Pattern/Incident logging, kept separate
- Projects: Critical (2) / Development (6) / Sleeping tiers with progress
- Cycle: calendar-month grid, Plan Ahead with per-day template override
- Lunar: cycle display
- Review: scoped At a Glance, Value Audit, Practice Consistency with
  performance correlation, Vision Check, Behavior breakdown, Project Pulse,
  Idea funnel
- Settings: Day Shape Templates, Weekly Default, Accountability, Backup
- Real on-device persistence (survives closing the app)
- Installable as a Progressive Web App (offline-capable via service worker)

## What's NOT in this build yet

- **Guide content is placeholder.** The tab exists; the real worked-example
  content per screen hasn't been written.
- **The 6 drafted 12-pair definitions** (Investment/Expense, Closing/Opening,
  Strategy/Tactic, Vital/Urgent, Building/Maintaining, Directing/Drift) are
  still marked "pending sign-off" in the Log screen, same as in the preview.
- **No migration tool** from the old PC-EOS or 60D-POS data — this is a
  fresh start, not an import.
- **No calendar sync or notifications** — this was flagged as a known gap
  against other apps and hasn't been built.
- **Today's Execution timetable is illustrative sample data**, not yet wired
  to automatically resolve from whatever you plan in Cycle for the real
  current day — Plan Ahead saves correctly, but Home's timetable doesn't
  yet pull from it automatically. Worth flagging as the next real fix.

## How to install it on your phone via GitHub

1. Create a new GitHub repository (public, so GitHub Pages can serve it free).
2. Upload every file in this folder to the repository root.
3. In the repo, go to **Settings → Pages**, set Source to your main branch,
   root folder, and save.
4. GitHub gives you a URL like `https://<yourname>.github.io/<repo>/` —
   open that on your Android phone in Chrome.
5. Tap Chrome's menu → **Add to Home screen** (or you'll see an automatic
   "Install app" banner). That installs it like a real app icon.

Every time you want to update it, replace the files in the repo with a new
build — the service worker will pick up the change next time the app opens
with a connection.
