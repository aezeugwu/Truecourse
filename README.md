# TrueCourse v0.11.0

*Observe → Capture → Learn → Change*

A personal cycle and execution app, the successor to PC-EOS and 60D-POS. It runs
on your phone as an installable web app, keeps everything on that phone (no
account, no server), and is built to keep working without a connection after the first load.

Version 0.11.0 · built 2026-10-02 · the version number is shown at the bottom
of **Settings**.

---

## The 11 tabs

| Tab | What it's for |
|---|---|
| **Home** | Today at a glance: the current block, today's schedule (tap a Critical or Development block to log it), your intention with **Breathe & reconnect**, the missed-block banner, live Day Score / Execution Ratio / Alignment Score, Tomorrow, the project pipeline. **Edit times / projects ›** changes today's schedule. |
| **Incubator** | Capture ideas, park them, and promote one to Critical, Development or Sleeping when there's room. Each idea records the date you captured it. |
| **Practice** | A ◀ ▶ date bar, then four sections: **Morning** (your ONE priority, phase, check-in), **Afternoon** (midday pulse, check-in), **Evening** (check-in plus 8 reflection questions), **Alignment** (see below). Everything saves as you type. |
| **Log** | **Block Activity**: pick a day and a block, mark Completed or Partial, set the real time, write what you did, move progress, tag it against the 12 pairs. **Pattern / Incident**: catch what pulled you off track or what you noticed. |
| **Journal** | A read-only feed of what you actually recorded, newest day first: work, patterns, practice, ideas, and blocks that were scheduled but never logged. |
| **Projects** | Critical (max 2), Development (max 6), Sleeping. Progress with − and + buttons. Tap a project for its objective, why it matters, notes, and Mark progress on a chosen date. Idle for 14 days shows as stagnant. |
| **Cycle** | A 30-day cycle you control, independent of the calendar month and the moon. Tap any day to set its template, projects and block times. |
| **Lunar** | The real moon phase and lunar day (display only). |
| **Review** | Scope by Day, Week, Cycle, Lunar or All. Scores, vision check, practice consistency, alignment practice, body baseline, what's draining you, environment audit, category breakdown, project pulse, idea funnel. |
| **Guide** | Every screen explained with examples, the 12 pairs, and the full 10 steps (last entry). |
| **Settings** | Cycle start/reset, **Day hours**, templates and weekly defaults, accountability and your Cycle Commitment, Google Calendar sync, Backup. |

---

## Rules worth knowing

- **Saving.** Practice, Projects and most fields save the instant you type or tap. There is no Save step to forget. (Block Activity and Pattern entries save when you tap their button.)
- **Filling in a missed day.** The ◀ ▶ date bar works in **Practice**, **Log → Block Activity** and **Log → Pattern / Incident**. **Projects → Mark progress** and **Incubator** take a date. Practice, Block Activity and Pattern entries filled in later are marked "logged later". You can never log into the future.
- **A new day.** If the app stays open past midnight, it refreshes itself when you return to it. Nothing is lost.
- **Choosing your hours.** Settings → Day hours sets when the day starts, how long Critical and Development blocks and lunch last, and when Evening Practice starts. To change one day, tap it in Cycle. To change today, use **Edit times / projects ›** on Home. Blocks are always listed in time order.
- **History is never rewritten.** Anything you've logged or marked done keeps the time it was logged at, whatever you change later.
- **Progress control.** − and + move it 5% a tap, so a stray touch can't jump it to 100%. Tap the number to type an exact value. The "last moved" clock only restarts when progress goes *up*.
- **Your Cycle Commitment.** Mark your ONE priority "Abandoned" on 3 or more days in a cycle and Home shows your stake back to you until you acknowledge it. Nothing is charged or locked.
- **Compress remaining schedule** (Home, after missed blocks) saves its new times, so a later change can't undo it.

---

## Alignment: the ten steps

Built from your summary of *How to Talk to the Universe*. The app does **not**
claim the book's explanation is true. It records the practices and shows, from
your own history, whether days with them look different.

| # | Step | Where it lives |
|---|---|---|
| 1 | Limiting beliefs | Practice → Alignment → *Beliefs I'm rewriting* → + Add a belief |
| 2 | Replacement beliefs | Same form. Shows on Practice → Morning and Evening with **I read it**, and on Home |
| 3 | What + Why + Feeling | Practice → Alignment → *Your intention* (also on Home) |
| 4 | Gratitude | Practice → Alignment → *Morning alignment* (3 gratitudes + one thing on its way; Quick mode) |
| 5 | Future-self decisions | Log → Pattern / Incident → + why / effect / link to project |
| 6 | Visualization | Alignment → Start 5-minute visualization (Quick = 2 min); ends by showing your obstacle and plan |
| 7 | Curate your environment | Review → *What's draining you* and *Environment audit* (once per cycle; Home reminds you) |
| 8 | Anchors | Home → *Your intention*: **Breathe & reconnect** (30 s) and **Lock-screen picture** |
| 9 | Body baseline | Alignment → four taps; Review compares with your Day Score |
| 10 | Detachment and reset | Pattern log "What is this asking me to adjust?" and the **2-minute reset** (Home banner, Alignment → Tools) |

Review compares your Day Score on days you did a practice against days you
didn't, **using finished days only**. It shows "not enough days yet" until both
kinds exist, and it labels the result as your own history, not proof of cause.
The lock-screen picture is saved to your Downloads; you set it as wallpaper
yourself. Timers count from the clock, so a locked screen doesn't throw them
off, but the buzz at the end may not fire while locked.

---

## Your data and backup

Everything is stored in this phone's browser storage. Clearing the browser's
site data **deletes it**, so export a backup first.

**Settings → Backup → Export JSON** saves a file containing: templates and weekly
defaults, day plans (including per-block times), project progress and
last-progress dates, projects, ideas, triggers, your intention, accountability,
logs, practice entries, day hours, beliefs, and environment audits.

**The backup does NOT include** (restoring on a new phone will lose these):

- **Each past day's schedule record** (which blocks were Completed or Partial that day). Your logged entries *are* saved, but the Day Score history that Review uses to compare days, and the Journal's "marked done, no details" lines, are not.
- **Your cycle start date** (the cycle would restart from the day you restore).
- **Your Google Client ID** (type it in again).

The text on the Backup card ("One export covers every store…") overstates this.
It is listed under Known gaps below.

---

## Updating the app

Each release changes **three files**: `app.js`, `sw.js`, `VERSION.txt`.

1. In your GitHub repository, upload those three over the old ones (same names).
2. Commit, wait about a minute for GitHub Pages to redeploy.
3. On your phone, fully close TrueCourse (recent apps → swipe it away) and reopen it. Do it twice if the first time doesn't show the change.
4. Check **Settings → bottom of the page**. It must show the new version number. If it shows an older one, your phone is still running a cached copy.

Never clear site data to force an update; it erases your data. Export first.
`sw.js` must change in every release (its version label is what tells the phone
there is something new), which is why it is always one of the three.

## First-time install

1. Create a public GitHub repository.
2. Upload **all 9 files** in this folder to the repository root, loose, not zipped.
3. Settings → Pages → Source: your main branch, root folder → Save.
4. Open the GitHub Pages address on your phone in Chrome.
5. Chrome menu → Add to Home screen.

## The files

| File | Purpose |
|---|---|
| `index.html` | The page shell. Also loads Google's sign-in library for Calendar Sync. |
| `app.js` | The entire app. |
| `sw.js` | Makes it installable and available offline. Its version label changes every release. |
| `manifest.json` | Install details: name, colors, icons. |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` | App icons. |
| `VERSION.txt` | Release notes for the latest version. |
| `README.md` | This file. |

---

## Known gaps (not done, or not working yet)

**Controls that do nothing yet**
- **Settings → Practice targets** (Wake target, Bedtime): the times are not saved or used anywhere. Day hours now covers when your day starts.
- **Settings → Alerts** ("Flag intent/actual mismatches on Home"): the checkbox does not change anything. The flag on Home appears whenever your intent and actual tags differ, whatever this box says.

**Data that is not real yet**
- **Review → Value Audit**: the 12 per-pair bars and the line "Where your B-time went" are sample values, not your tag history. Execution Ratio and Alignment Score near the top *are* real.

**Not built**
- Appointment blocks that flag any work block they overlap. The editor only refuses a block that ends before it starts, so two blocks can share a time.
- A Discard action for Incubator ideas.
- Backfill on Lunar (it has nothing to enter).
- A migration tool from PC-EOS / 60D-POS data.
- Syncing between devices.
- Two-way calendar sync.

**Unverified**
- **Offline use.** The app's files are cached on the phone, so it should open without a connection. That has not been tested on a real phone.
- **Google Calendar sync** is a one-way push of today's Critical and Development blocks. It has never been tested against a real Google account (it needs a Client ID; steps are in the Guide). It only syncs while the app is open.

**Minor**
- The Backup card's wording overstates what is exported (see above).
- Backup files carry an internal label of "0.3.0". Restoring never reads it, so it is harmless.
- If the app wasn't opened on a past day, that day's schedule is rebuilt from your templates and hours as they are now.

---

## Version history

| Version | What changed |
|---|---|
| 0.11.0 | **Alignment**: all ten steps (intention, gratitude, visualization timer, beliefs, body baseline, anchors, resets, environment audit). Comparisons use finished days only. |
| 0.10.0 | **Day hours** and per-block times for any day, including today. Today's schedule follows your plan. Compress now sticks. |
| 0.9.1 | **Journal** tab. |
| 0.9.0 | Fill in a missed day everywhere. − / + progress control. The app refreshes on a new day. |
| 0.8.1 | The real version number in Settings. |
| 0.8.0 | Pattern / Incident rebuilt to match PC-EOS: duration, why, effect, project links, Today's events, editable triggers. |
| 0.7.4 | Category definitions in the Guide. Review's category chart and idea funnel use real data. |
| 0.7.3 | "Open full Review" works. |
| 0.7.2 | Fixed Log crashing when there were no Critical or Development projects. |
| 0.7.1 | Practice fields wired up. The app fills the screen. |
| 0.7.0 | The 30-day cycle became independent of the calendar. |
| 0.6.1 | Fixed updates not reaching the phone. |
| 0.6.0 | Soft stake enforcement. Google Calendar sync. |
| 0.5.0 | All 12 value pairs finalized with your own examples. |
| 0.4.0 | Project detail page. |
| 0.3.x | Incubator, add projects, backup, managed triggers, adaptive day, full Guide. |
| 0.2.0 | Real computed scores, schedule, moon and stagnation. |
| 0.1.0 | First installable version. |
