# Power Scale Ladder

An interactive teaching tool that shows how big electrical quantities really are. People hear "50 kW", "700 MWh" or "11 kV" but have no feel for the size. This tool turns the numbers into things you can picture: people pedalling, kettles, diesel generators, power stations, pole heights and copper thickness.

**Live demo:** https://YOUR-GITHUB-USERNAME.github.io/power-scale-ladder/

## What it does

| Section | What you see |
|---|---|
| Lecture scenes | 8 ready-made teaching moments. One tap sets up every section and shows a talking point. Arrow keys move between scenes. Projector mode enlarges everything. |
| 1 · Choose a power | Any value from 1 W to 10 GW, by typing, sliding or picking a preset. |
| 2 · That is about | The power in everyday equivalents (bulbs, people pedalling, kettles, clinics, generators, Bumbuna Hydro, nuclear reactors). |
| 3 · Picture it | The power drawn as a grid of icons: pedallers, kettles, generators or hydro dams. |
| 4 · The ladder | A log scale where each step is 10× bigger, with familiar examples marked. |
| 5 · Compare two powers | Side-by-side bars and the ratio, for lectures ("this is 10 kW, this is 50 kW"). |
| 6 · Power × time = energy | kW is speed, kWh is distance. Energy shown as pedalling hours, litres of diesel, phone charges and lifting height. |
| 7 · Voltage | 1.5 V to 765 kV, with where each level is used, insulator discs, pole height and the keep-out distance, drawn to scale. |
| 8 · Current | 1 mA to 100 kA, with effects on the human body, copper size needed (drawn to scale) and kettle equivalents. |
| 9 · Same power, different voltage | Why grids use high voltage: current and copper needed for the same power at 230 V up to 400 kV. |

Examples are drawn from Sierra Leone and Bangladesh (Bumbuna Hydro, the 225 kV CLSG line, 230 V supply, 400 kV national grid).

## How to run

It is a single HTML file with no build step and no install.

- Open `index.html` in any browser, or
- Visit the GitHub Pages link above.

Works on phones, laptops and projectors.

## Assumptions and limits

All figures are typical round values for teaching, not design data.

- Person pedalling: about 100 W sustained. Diesel generator: about 3 kWh of electricity per litre. Lifting: E = mgh, g = 9.81 m/s².
- Keep-out distances use the US OSHA rule for unqualified workers near overhead lines (3.05 m up to 50 kV, plus 10.2 cm per 10 kV above). Local rules differ.
- Copper sizes are approximate single-cable ratings in free air. Above about 460 A the tool assumes a copper busbar at 1.5 A/mm².
- Body-current effects are for 50 Hz AC and vary between people.

## Built with

Plain HTML, CSS and JavaScript (Canvas for drawings). Fonts from Google Fonts.

## Roadmap

- Offline install as a phone app (PWA)
- Local safety standards for Sierra Leone and Bangladesh
- Krio and Bangla translations
- Quiz mode for students
