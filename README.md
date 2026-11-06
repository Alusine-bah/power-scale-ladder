# Power Scale Ladder

An animated teaching tool that shows how big electrical quantities really are. People hear "1 MW", "700 MWh" or "11 kV" but have no feel for the size. This tool lets you watch it: homes switching on across a city at night, current flowing down a line until the wire glows and melts, and energy "fired" at a target to see the impact.

**Live demo:** https://alusine-bah.github.io/power-scale-ladder/

## Three scenes

**1 · Light a city.** A satellite-style night map. Choose any power from 1 W to 2 GW and watch homes light up, from LED bulbs inside one house to a whole city. The camera pulls back as the power grows, so a village shrinks to a dot next to a city, the way a river looks next to an ocean. A scale bar shows real distance.

**2 · Current on a wire.** Poles and towers drawn to scale with a person beside them, and a live conductor with charge flowing along it. Pick the voltage (230 V to 400 kV). For the same power, low voltage pushes a huge current: the wire overheats, glows, sags and melts. High voltage needs only a small current. The scene also shows heat lost per kilometre and the keep-out distance around the line.

**3 · Impact test.** Run the chosen power for a minute, an hour, a day, a month or a year, then aim it at a target:
- **Boil water:** containers fill and steam, from cups to Olympic pools.
- **Lift a car:** a 1.5-tonne car rises past a house, a 10-storey building, Mount Bintumani, a cruising jet, the edge of space and the Moon, with the camera zooming out as it climbs.
- **Diesel it replaces:** the fuel a generator would burn to make the same electricity.

## How to run

A single HTML file with no build step: open `index.html` in a browser, or use the live demo. Works on phones, laptops and projectors.

## Assumptions

Teaching values, not design data.
- 1 home ≈ 1 kW average evening demand. Homes on a 15 m grid.
- Wire scene uses one 240 mm² copper conductor (about 400 A, 0.0754 Ω/km) at every voltage so the effect of voltage is visible. I = P/(√3·V) for three-phase.
- Keep-out distances: US OSHA rule for non-electrical workers near overhead lines.
- Water heated from 25 °C to 100 °C (c = 4186 J/kg·K). Lift: E = mgh. Diesel generator ≈ 3 kWh per litre. No losses.

## Built with

HTML, CSS and JavaScript with Canvas 2D animation. No libraries.

## Roadmap

- Arc-flash scene: what happens when a ladder gets too close to 11 kV
- Lecture mode with guided scenes
- Krio and Bangla translations
- Offline phone app (PWA)
