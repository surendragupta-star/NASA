# Crew Health Console

Health monitoring software that helps astronauts check their own health on long space missions and decide what to do next.

Built by **Team SURENDRA** for the challenge **Create Health Monitoring Software for Astronauts on Space Missions**.

## Repository contents

| Path | What it is |
|---|---|
| `index.html` | The Crew Health Console app (single file) |
| `presentation/index.html` | 7-slide demo presentation with speaker notes |
| `presentation/source/` | Slide source files (HTML, CSS, JSON) |
| `docs/SUBMISSION.md` | Submission text: summary, project details, data and resources |

## Run it

The whole app is one file, `index.html`. No build step, server or install is needed.

- Open `index.html` in any modern browser, or
- Enable GitHub Pages for this repository (Settings → Pages → deploy from the `main` branch) and open the published URL.

The app opens with 23 days of **sample data** from a fictional crew member so every feature has something to show. Select **Start my own log** to clear it. Your entries are stored only in your browser (`localStorage`).

## Features

- **Interactive body map:** clickable regions for brain, eyes, lungs, heart, metabolism, and bones and muscles, plus immune system and radiation. Each is colored green, amber or red and explains what the system does, how spaceflight affects it, self-care steps and when to contact a flight surgeon.
- **11 indicators:** resting heart rate, blood pressure, blood oxygen, body temperature, blood glucose, sleep, mood, exercise, fluid intake, daily radiation dose and body mass, each with a status badge, a sparkline and a 21-day trend chart with the target range shaded.
- **Guided logging:** a "How to measure" note for every field and a symptom checklist with red-flag symptoms marked for escalation.
- **Flags and actions:** out-of-range readings with a next step, plus multi-day trend checks (sleep shortfall, rising blood pressure, low exercise, falling body mass, overdue eye check, cumulative dose against NASA's 600 mSv career limit).
- **Mission environments:** low Earth orbit station, deep-space transit, lunar base, lunar rover and Mars base. Each adjusts expected radiation dose, gravity, bone-loss estimate, signal delay and escalation advice.
- **Daily routine and gamification:** a timed checklist that completes itself as data is logged, with XP, levels, streaks and badges.
- **Flight surgeon report:** a one-click text summary of the day's vitals, symptoms, flags and system status.
- **Hazard primer:** NASA's five hazards of human spaceflight and the indicators that track each.

## How it works

Plain HTML, CSS and JavaScript with no frameworks or dependencies besides Google Fonts. It works offline, which suits spacecraft with limited bandwidth and long communication delays. Each reading is graded against a target range and a caution range; each body system takes the worst status among its readings, symptoms and trend flags. The body map and charts are drawn with SVG. Light and dark themes follow the system setting.

## Data sources

- NASA Human Research Program: the five hazards of human spaceflight
- NASA-STD-3001: 600 mSv career radiation limit
- NASA research on spaceflight-associated neuro-ocular syndrome (SANS), bone loss in microgravity (about 1–1.5% per month) and exercise countermeasures
- Curiosity rover RAD instrument: Mars surface dose of about 0.64 mSv/day
- Chang'e 4 lunar lander (Zhang et al., *Science Advances*, 2020): lunar surface dose of about 1.4 mSv/day

## Limitations

This is decision support for crew self-assessment, not a medical diagnosis. Target ranges are simplified general adult reference values; a real deployment would use each crew member's baseline and limits set by their flight surgeon. Bone-loss rates in partial gravity are not yet measured, so the Moon and Mars rates are assumptions.
.
