# MarbleRacing Manager

Run your own marble racing team. Build up your marbles, pick two to race, and chase the team title through four series, from the Clubman Series up to the World Marble Championship.

**Play:** open `index.html` in a browser (needs an internet connection for the 3D engine, physics and fonts). Keep the other files next to it: they are the podium trophies, the Lake Village scenery and the music.

## How to play
- **Race Day** — your home screen: next track, your racing marbles, standings and the start button.
- **Garage** — two tabs. **Marbles:** pick two to race and run workshop sessions; every session is a short minigame, and the grade (Perfect, Good, OK, Miss) sets how much the stat goes up. **Tools:** upgrade each tool for bigger gains and an easier minigame.
- **Shop** — the marble run gacha tower for new marbles and items. Every machine has a guarantee.
- **Bet** — stake coins on who wins the next race.

Each season has 6 races. Win the team title to move up a series.

## Stats
| Stat | What it does |
|---|---|
| SPD (speed) | Pace on straights |
| GRP (grip) | Pace on sand, hairpins and chicanes |
| STA (stability) | Pace on ice, pegs, slalom and banked corners, and fewer wobbles there |
| Toughness | Lower crack chance and less wear |
| Weight | Set by the material: **Light** is quick to speed up and nimble, **Heavy** keeps its speed, wins bumps and is good on sand |

Each marble shows a **crack risk** (Low, Medium, High). Only a High-risk marble can shatter, and you are warned before racing it.

## Tracks
Lake Village · Sandbanks GP · Snowhill County · Mokuzai GP · Euphoria GP · Noman Islands · Plinko City · Lembah Highlands

## Tech
A single HTML file. 3D races use [three.js](https://threejs.org) (WebGPU with WebGL2 fallback) and [Rapier](https://rapier.rs) physics, with a 2D fallback race. Saves are kept in the browser (localStorage). English and Bahasa Melayu. Light and dark mode.

## Files
- `index.html` — the whole game
- `trophies.json` — 3D podium trophies (gold, silver, bronze, champion)
- `scenery-lake.json` — Lake Village house, jetty and boat
- `music-*.mp3` — menu and race music (the music button in the top bar cycles On, Menus only, Off)
- `favicon.svg` — browser tab icon
- `netlify.toml` — Netlify settings (no build step)
- `CHANGELOG.md` — what changed in each version
