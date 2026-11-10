# Pixel Keep

An offline, single-file pixel-art tower defense game. Open `index.html` in any modern browser; it works straight from `file://`. There are no dependencies, no network requests and no build step, and the whole game is one file of about 100 KB.

## Features
- **10 campaign levels**, each with its own map and theme and a smooth difficulty curve. Bosses appear on levels 4, 7 and 10 (Slime King, Iron Golem, Dread Lich).
- **8 towers:** Arrow, Cannon, Frost, Gold Mine (economy and damage aura), Sniper, Tesla, Missile (anti-air) and Flame. Each has 3 upgrade tiers, 4 targeting modes, and can be sold back.
- **12 enemy types:** flyers, armored, magic-resistant, splitters, healers, shields, blinkers and sprinters.
- **Survival mode** (available from the start): procedural, endlessly scaling waves with periodic bosses. Every tower is available in Survival. Your best wave is saved.
- **Meta-progression:** stars earned per level buy permanent upgrades. In each run you can also spend gold on Research.
- **Saves to localStorage:** unlocks, stars, upgrades, survival best and options.
- **Responsive layout:** landscape uses a side panel. In portrait the map is transposed into a vertical layout and the controls sit in a thumb-reach bottom strip. Touch and mouse are both supported.
- All sprites are drawn in code and all sound effects and chiptune music are synthesized with the Web Audio API.

## Controls
Mouse or touch: pick a tower from the palette, then tap a grass tile. On touch screens, tap once to preview and tap the same tile again to build. Tap a built tower to upgrade, sell or change its targeting.

Optional keys: `1-8` towers · `9` research · `N` next wave · `F` speed · `Space` pause · `U` upgrade · `S` sell · `T` targeting · `Esc` cancel.

## Tweaking
All balance data lives near the top of the script: `TOWERS`, `ENEMIES`, `LEVELS` (paths and wave strings such as `"orc 6 1.2"` for type, count and spawn interval), `PERKS` and `RESEARCH`.
