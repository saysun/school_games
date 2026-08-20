# School Games

Two web-based HTML games for a 7-year-old learning English past tense, built from the homework worksheets (Units 1–8).

Both games are **single-file, vanilla HTML/CSS/JS** — no build step, no dependencies, no install. Open the HTML file in any modern browser (desktop or phone) and play.

## Games

### 🎯 Tense Quest (`tense-quest.html`)

**Tap-to-match game** — 36 rounds, one verb per round.

- Top: present-tense verb (e.g. `see`)
- Bottom: 2/3/4 choice buttons with past-tense forms
- Kid taps the correct past tense → sparkle + green flash + example sentence reveals
- Wrong taps → red shake + "Try again!" + correct answer highlighted
- Difficulty: **Easy** (2 choices) / **Medium** (3 choices, default) / **Hard** (4 choices)
- **Silent** — no audio
- End screen has a **Words to Practice** review listing every verb missed with what they picked

### 🧩 Tense Match (`tense-match.html`)

**Tap-to-clear tile game** — clear all 36 tiles.

- Top: present-tense verb
- Below: a 6-column grid of all 36 past-tense tiles (one per verb)
- Kid taps the matching past tense → tile spins away (0.5s animation), example sentence reveals, next verb appears
- Wrong taps shake the tile (no penalty — tiles stay)
- Win when every tile is cleared
- **Silent** — no audio
- End screen rates the run on wrong taps: 0 = Perfect, ≤3 = Awesome, ≤8 = Good job

## Verbs covered (all 36 from homework)

**Sheet 1:** see→saw, sit→sat, skip→skipped, slip→slipped, smile→smiled, squirt→squirted, stop→stopped, talk→talked, tell→told, think→thought, try→tried, waggle→waggled, wander→wandered, watch→watched, wear→wore

**Sheet 2 (Unit 1–8):** blow→blew, carry→carried, clean→cleaned, cry→cried, do→did, eat→ate, fall→fell, get→got, hide→hid, huff→huffed, hug→hugged, kneel→knelt, look→looked, make→made, open→opened, prowl→prowled, puff→puffed, run→ran, say→said, scratch→scratched, scrape→scraped

## How to run

Just open either file in a browser:

```bash
# Desktop
xdg-open tense-quest.html   # or double-click

# Phone — scan a QR code pointing at the file's URL, or
# host via any static server:
python3 -m http.server 8000
# Then visit http://<your-ip>:8000/tense-quest.html
```

## Built with

- Pure HTML5 + CSS3 (flexbox, grid, animations)
- Vanilla JavaScript (no frameworks, no build)
- Web Speech API was previously used but has been removed — games are now silent

## Files

| File | Size | Purpose |
|------|------|---------|
| `tense-quest.html` | ~24 KB | Tap-to-match game (3 difficulty modes) |
| `tense-match.html` | ~21 KB | Tile-clear game |
| `README.md` | this file | Documentation |