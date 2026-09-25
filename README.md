# TrueCourse v0.7.2

Personal Cycle & Execution OS — the merged successor to PC-EOS and 60D-POS.

## What's fixed

**Log was crashing silently.** If you had zero Critical and zero
Development projects — easy to reach while testing Add/Remove — the
Log screen tried to default to "the first available project" and hit
a hard error with nothing shown on screen, which just looked like the
page refusing to open. Fixed: it now shows a clear message and points
you to Projects or the Incubator instead. A second, less likely version
of the same kind of crash (an empty schedule for the day) was also
guarded against while this was being fixed.

**Confirmed by design:** Morning and Afternoon in Practice have no
Save button on purpose — everything there saves the instant you
interact with it, same as most of the app. Evening keeps its Save
button as a closing confirmation for a screen with several fields.

## What's real (cumulative)

Everything from v0.2.0 through v0.7.1.

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
