# TrueCourse v0.8.1

Personal Cycle & Execution OS — the merged successor to PC-EOS and 60D-POS.

## What changed in v0.8.1

The Settings footer now shows the real version (it had said "v0.3" for many releases), so you can confirm at a glance which version your phone is running: Settings → bottom of the page → "TrueCourse v0.8.1".

## What changed in v0.8.0

The Pattern/Incident log is rebuilt to match your original PC-EOS
"Capture a loop" screen (see VERSION.txt for the full list): duration
chips, optional category chips, the expandable why / effect / project
link section, "Add to log" with a "Today's events" list underneath,
editable saved triggers, and a ◀ ▶ date bar for backfilling a missed day.

## Still illustrative — please don't trust these yet

- **Value Audit (Review)**: the 12 per-pair bars AND the line beneath
  them ("Where your B-time went: Reactive (9)…") are sample values, not
  your real tag history. Execution Ratio and Alignment Score above it
  ARE real.

## Still missing compared with your original PC-EOS

- **Backfilling a past day on Practice (Morning/Afternoon/Evening) and
  Lunar.** The date bar only exists on the Pattern log so far; Practice
  still always writes to today.
- **Incubator: no Discard** action for an idea.
- The original **Dashboard** and its "top recurring loops" view. Home
  and Review cover much of it, but recurring triggers/loops aren't
  surfaced yet, even though the data to do it is now being captured.

## Deliberately not built

Migration tool, cross-device sync, true two-way calendar sync.

## How to update your installed app

Replace all 9 files. Commit, wait a minute for GitHub Pages to
redeploy, then fully close TrueCourse (swipe it away from recent apps)
and reopen it, possibly twice.

## First-time install (for reference)

1. Create a public GitHub repository.
2. Upload every file in this folder to the repo root, loose, not zipped.
3. Settings → Pages → Source: your main branch, root folder → Save.
4. Open the GitHub Pages URL on your phone in Chrome.
5. Chrome menu → Add to Home screen.
