# TrueCourse v0.7.1

Personal Cycle & Execution OS — the merged successor to PC-EOS and 60D-POS.

## Two real bugs fixed in this version

**1. Practice tab was partly non-functional.** The Morning phase
selector (Start/Build/Finish/Review/Reset) never responded to taps —
"Build" was hardcoded as permanently selected in the code, with no
click handler at all. The "What must be true by tonight?" field and
all 8 Evening review questions were also never wired to anything, so
nothing typed there was ever saved. All of this is fixed now — same
auto-save-as-you-go pattern as the rest of the app.

**2. The real app was showing a decorative phone-mockup frame.**
Every version since launch has rendered inside a fixed-width, black-
bordered box on a beige backdrop with a big dead empty area below it —
a frame that was only ever meant for previewing inside a chat
conversation, not for an actual installed app on a real phone. Fixed:
the app now fills the real device screen properly.

## What's real (cumulative)

Everything from v0.2.0 through v0.7.0, now with a fully functional
Practice tab and a properly full-screen layout.

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
