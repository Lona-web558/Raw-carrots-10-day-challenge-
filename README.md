# Raw-carrots-10-day-challenge-


# 10-Day Raw Carrots Challenge

A single-file web app that tracks a 10-day "eat a raw carrot" habit challenge, with progress saved locally in the browser.

## Features
- 10 tappable day cards — click to mark a day complete/incomplete
- Live progress bar and "Day X of 10 complete" counter
- Current streak tracker (consecutive completed days from Day 1)
- Completion message when all 10 days are done
- Reset button to start the challenge over
- Data persists via browser `localStorage` — no backend, no build step, no account needed

## Tech stack
- HTML5
- CSS3 (custom styles, carrot/leaf color theme)
- Bootstrap 5.3 (via CDN) for layout and grid
- Vanilla JavaScript for state and interactivity

## Files
- `carrot-challenge.html` — the entire app (markup, styles, and script in one file)

## Running it
Just open `carrot-challenge.html` in any modern browser. No server or installation required.

## Data storage
Progress is stored under the `localStorage` key `carrotChallenge10Day` as a JSON array of 10 booleans (one per day). This is:
- Local to the specific browser and device — it won't sync across devices
- Cleared if the user clears their browser's site data
- Reset manually anytime via the in-app "Reset Challenge" button

## Customizing
- Change `TOTAL_DAYS` in the script to adjust the challenge length
- Colors are set via CSS variables (`--carrot`, `--carrot-dark`, `--leaf`) near the top of the `<style>` block
