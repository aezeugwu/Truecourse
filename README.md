# TrueCourse v0.6.0

Personal Cycle & Execution OS — the merged successor to PC-EOS and 60D-POS.

## What's real (cumulative)

Everything from v0.2.0 through v0.5.0, plus:

- **Soft stake enforcement.** Practice → Afternoon's pulse (On Track /
  At Risk / Abandoned) is now genuinely wired to real data — it was a
  decorative, non-functional control before this version. Mark
  "Abandoned" 3 or more days within a calendar-month cycle, and Home
  shows a full-screen confrontation with your own Cycle Commitment text
  until you tap "I see it." Resets each new day. No money moves, no
  feature gets locked — this is detection and confrontation, not
  punishment, by deliberate design choice.
- **Google Calendar sync (one-way push).** Settings → Calendar Sync:
  paste a Google OAuth Client ID (steps to get one are in the Guide's
  new "Calendar Sync" entry), tap Connect, then Sync today's blocks —
  your Critical and Development blocks become real events in your
  Google Calendar, so Google's own reminders handle notifying you.
  Runs entirely client-side, no server required — but that also means
  it only syncs while the app is open; it cannot push while your phone
  is asleep or the app is closed.

**Important — please test this part yourself:** the build environment
this was created in has no internet access, so the actual OAuth
handshake and real Google Calendar event creation could not be
verified end-to-end before shipping. Everything that could be tested
without internet (disabled states, graceful failure when the library
can't load, no crashes) was tested and passed. The live connection
needs to be tried on your actual phone.

## What's NOT in this build yet

- **Value Audit's per-pair bars (Review)** are still illustrative — the
  headline Execution Ratio and Alignment Score above them ARE real.
- **No migration tool** — deliberately dropped, not worth building.
- **No cross-device sync** — deliberately on the back burner.
- **No true two-way calendar sync** — changes made in Google Calendar
  itself don't flow back into TrueCourse. That would need a real
  server; this one-way version deliberately doesn't.

## How to update your installed app

Replace `app.js`, `index.html`, `VERSION.txt`, and `README.md` in your
GitHub repo (`index.html` changed this time — it now loads Google's
sign-in library). `manifest.json`, `sw.js`, and the three icons are
unchanged. Commit, wait a minute for GitHub Pages to redeploy, reopen
the app — your existing data is untouched.

## First-time install

1. Create a public GitHub repository.
2. Upload every file in this folder to the repo root — loose, not zipped.
3. Settings → Pages → Source: your main branch, root folder → Save.
4. Open the GitHub Pages URL on your phone in Chrome.
5. Chrome menu → Add to Home screen.
