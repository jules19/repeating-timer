# Practice Timer

A simple repeating interval timer for piano practice, built as a single-page
web app for iPhone and iPad.

**Live app:** https://jules19.github.io/repeating-timer/

## What it does

Pick an interval (1, 1½, 2, 3 or 5 minutes, or any custom length), tap
Start, and practice. When the timer expires it plays a gentle bell chime,
then automatically resets and repeats — forever, until you tap Pause or
Reset. Use it to switch exercises or move to the next section of a lead
sheet without touching the phone.

## Features

- One-tap preset durations plus a custom duration in minutes (decimals OK, e.g. `2.5`)
- Repeats endlessly with a cycle counter so you know how many rounds you've done
- Pleasant two-note bell chime synthesized with the Web Audio API — no audio files, works offline
- Keeps the screen awake while running (Wake Lock API) so iOS never suspends the timer
- Drift-free timing based on real timestamps, not tick accumulation
- Remembers your last-used duration
- No build step, no dependencies — one `index.html`

## Tips for iPhone/iPad

- Open the site in Safari, tap **Share → Add to Home Screen** to get a
  full-screen app without browser chrome.
- Sound starts working after your first tap on Start (an iOS requirement) —
  make sure the ring/silent switch isn't muting Safari if you don't hear the chime.

## Hosting

Deployed to GitHub Pages automatically by the workflow in
`.github/workflows/deploy-pages.yml` on every push.
