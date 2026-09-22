# TrueCourse v0.6.1

Personal Cycle & Execution OS — the merged successor to PC-EOS and 60D-POS.

## Important: read this before updating

Every previous update told you `sw.js` was "unchanged, no need to
re-upload." That was true about its content, but it was the wrong
guidance — browsers only check for a new service worker when that
file's bytes actually differ, so `sw.js` never being touched meant your
browser had no reason to ever notice any of the updates in between.
Your phone was likely still running the very first version this whole
time. This version fixes that by changing `sw.js` for the first time
since launch. From now on, `sw.js` gets bumped with every release.

## What's real (cumulative)

Everything described in every version from v0.2.0 through v0.6.0 —
real computed scores, Idea Incubator, Adaptive Day Engine, working
Export/Import, Project detail page, all 12 Value Audit pairs finalized
with your real business examples, soft stake enforcement, and Google
Calendar one-way sync. If you're updating from the original install,
you're likely about to see all of this appear at once, not just the
Incubator.

## What's NOT in this build yet

- Value Audit's per-pair bars (Review) are still illustrative.
- No migration tool, no cross-device sync, no true two-way calendar
  sync — all deliberate.

## How to update your installed app

Replace **all 9 files** — given how much was likely never actually
applied, do a full replace rather than trying to track partial diffs:
delete everything in the repo and upload these 9 fresh. Commit, wait a
minute for GitHub Pages to redeploy.

**Then, on your phone:** simply reopening the app may not be enough —
service workers can take a reload or two to actually switch over.
Close the app fully (swipe it away from recent apps), reopen it, and
if Incubator still isn't there, reopen it a second time. If it's still
missing after that, tell me and we'll troubleshoot further rather than
assume it worked.

## First-time install (for reference)

1. Create a public GitHub repository.
2. Upload every file in this folder to the repo root — loose, not zipped.
3. Settings → Pages → Source: your main branch, root folder → Save.
4. Open the GitHub Pages URL on your phone in Chrome.
5. Chrome menu → Add to Home screen.
