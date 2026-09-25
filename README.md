# TrueCourse v0.7.3

Personal Cycle & Execution OS — the merged successor to PC-EOS and 60D-POS.

## What's fixed

"Open full Review →" on Home did nothing when tapped — it had no click
handler at all, the same kind of oversight as the phase chips and
Evening fields fixed in v0.7.1. It now correctly opens Review. A full
scan of every button and tap-chip in the app was done afterward to
check for any others like it — none remain.

## What's real (cumulative)

Everything from v0.2.0 through v0.7.2.

## What's NOT in this build yet

- Value Audit's per-pair bars (Review) are still illustrative.
- No migration tool, no cross-device sync, no true two-way calendar sync.

## How to update your installed app

Replace all 9 files. Commit, wait a minute for GitHub Pages to
redeploy, then fully close TrueCourse (swipe it away from recent apps)
and reopen it — possibly twice.

## First-time install (for reference)

1. Create a public GitHub repository.
2. Upload every file in this folder to the repo root — loose, not zipped.
3. Settings → Pages → Source: your main branch, root folder → Save.
4. Open the GitHub Pages URL on your phone in Chrome.
5. Chrome menu → Add to Home screen.
