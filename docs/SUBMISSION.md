# Crew Health Console – Submission

**Team:** SURENDRA
**Challenge:** Create Health Monitoring Software for Astronauts on Space Missions
**Live demo:** https://surendragupta-star.github.io/NASA/
**Slides:** https://surendragupta-star.github.io/NASA/presentation/
**Code:** https://github.com/surendragupta-star/NASA

## High-level summary

Crew Health Console is an interactive tool that helps astronauts check their own health on long missions and decide what to do. Crew members log 11 indicators that can be measured in space (heart rate, blood pressure, blood oxygen, temperature, glucose, sleep, mood, exercise, fluids, radiation dose and body mass) along with symptoms, with simple measuring instructions for each. A clickable body map colors each system green, amber or red and explains how spaceflight affects it, what the astronaut can do, and when to contact a flight surgeon. Trend charts and flags catch slow problems such as sleep debt, rising blood pressure, low exercise and total radiation dose against NASA's 600 mSv limit. The tool adapts to the mission setting (station, deep-space transit, Moon, rover or Mars), adjusting expected radiation, gravity effects and signal delay; on Mars it tells the crew to act first rather than wait for the ground. A daily checklist with points, streaks and badges keeps health tasks a habit, and a one-click report summarizes the day for flight surgeons. It runs offline in a browser and is based on NASA Human Research Program data.

## Project details

### What it does and how it works

Each day the astronaut logs 11 health indicators measured with standard onboard equipment, plus any symptoms. Every field has a short "How to measure" note written for spaceflight. Each reading is checked against a target range and a caution range and colored green (Nominal), amber (Watch) or red (Act now). These results feed into:

- **Interactive body map:** brain, eyes, lungs, heart, metabolism, and bones and muscles, plus immune system and radiation exposure. Each region shows its worst current reading, symptom or trend, and explains what the system does, how spaceflight affects it, self-care steps and when to contact a flight surgeon.
- **Telemetry tiles and 21-day trend charts** with the healthy range shaded.
- **Flags and actions:** a specific next step for each out-of-range reading, plus multi-day trend checks (sleep debt, rising blood pressure, low exercise, falling body mass, overdue eye check, cumulative radiation dose).
- **Mission-aware guidance:** station, deep-space transit, lunar base, lunar rover or Mars base change the expected radiation, gravity, bone-loss estimate, signal delay and escalation advice.
- **Daily routine with rewards:** a timed checklist that ticks itself off as data is logged, with points, levels, streaks and badges.
- **Flight surgeon report:** a one-click text summary for the ground team.
- **Hazard primer:** NASA's five hazards of human spaceflight and the indicators that track each.

### Benefits

Fast self-assessment without medical training, early warning on slow declines, clear decisions on when to call the ground, built-in learning, better daily habits, consistent reports for flight surgeons, and offline operation suited to spacecraft networks.

### Intended impact

Give astronauts far from Earth the knowledge and confidence to look after their own health, so small problems are caught early and handled correctly. The same approach can help people in other isolated places such as Antarctic stations, submarines and analog missions.

### Tools and technologies

HTML5, CSS3 and JavaScript (no frameworks), SVG graphics, browser local storage, Google Fonts (Chakra Petch, IBM Plex Sans, IBM Plex Mono), Git and GitHub, and Claude (Anthropic) as an AI coding assistant. Runs in any modern browser on a laptop or tablet.

### Creativity

The body map is the dashboard; advice depends on where the crew is; trends matter as much as single readings; health tasks work like mission tasks; and the tool teaches as it monitors.

### Factors considered

What can be measured in space, NASA's five hazards, communication delay, users without medical training, mental health and privacy, limited computing resources, accessibility, safety and honesty about limits, and use of space agency data.

## NASA data and resources

- NASA Human Research Program – https://www.nasa.gov/hrp/
- NASA – The Human Body in Space – https://www.nasa.gov/humans-in-space/the-human-body-in-space/
- NASA Human Research Roadmap – https://humanresearchroadmap.nasa.gov/
- NASA – Why Space Radiation Matters – https://www.nasa.gov/missions/analog-field-testing/why-space-radiation-matters/
- NASA OCHMO Human System Standards (NASA-STD-3001) – https://www.nasa.gov/ochmo/hsa-standards/
- NASA OCHMO Technical Brief – Radiation Protection – https://www.nasa.gov/wp-content/uploads/2023/12/ochmo-tb-020-radiation-protection.pdf
- NASA OCHMO Medical Technical Brief – SANS – https://www.nasa.gov/wp-content/uploads/2024/02/ochmo-mtb-001-sans.pdf
- NASA OCHMO Medical Technical Brief – Bone Loss – https://www.nasa.gov/wp-content/uploads/2026/02/ochmo-mtb-013-bone-loss.pdf
- NASA Mars Science Laboratory Curiosity Rover – https://science.nasa.gov/mission/msl-curiosity/
- Hassler et al. (2014), Mars' Surface Radiation Environment Measured with the MSL Curiosity Rover – https://doi.org/10.1126/science.1244797
- Zeitlin et al. (2013), Measurements of Energetic Particle Radiation in Transit to Mars on the MSL – https://doi.org/10.1126/science.1235989

## Other data and resources

- Zhang et al. (2020), First Measurements of the Radiation Dose on the Lunar Surface (Chang'e 4, CNSA) – https://doi.org/10.1126/sciadv.aaz1334
- Google Fonts: Chakra Petch, IBM Plex Sans, IBM Plex Mono (SIL Open Font License) – https://fonts.google.com
- Claude by Anthropic (AI coding assistant) – https://www.anthropic.com/claude
- GitHub – https://github.com

## Limitations

Decision support, not diagnosis. Target ranges are simplified adult reference values; a real deployment would use each astronaut's baseline and limits set by their flight surgeon. Bone-loss rates in partial gravity are not yet measured, so Moon and Mars rates are assumptions. The lunar rover radiation dose is an estimate.
