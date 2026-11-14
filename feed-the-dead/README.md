# Feed the Dead: an Undead Drive-Thru

An offline, single-file pixel-art tower defense game. Zombies shamble through your restaurant toward the kitchen. Feed them junk food until they go **POP!**

Open `index.html` in any modern browser. There are no dependencies, no network requests and no build step.

## Features
- **10 restaurants:** Diner, Pizzeria, Taqueria, Food Court, Sushi Bar, Night Market, Drive-Thru Lot, Curry House, Rooftop Café and Stadium. Each has its own floor, furniture and aisle layout. Tables, plants and decor block building, so stations go on the marked floor tiles. Later levels have two entrances.
- **3 bosses:** Mall Cop Zombie (whistle stuns stations), Food Truck Zombie (spawns minions, armors up) and Zombie Celebrity Chef (summons fans, rewrites your menu, gets bodyguards, goes for an encore).
- **10 stations:** Burger Grill, Pizza Oven, Slushie Machine, Tip Jar, Boba Stand, Sushi Chef, Churro Cart, Taco Truck, Curry Pot and Espresso Bar. Each has 3 upgrade tiers, 4 targeting modes and sell-back.
- **Food tags and picky eaters:** foods are tagged MEAT, VEGGIE, SWEET, DRINK or SPICY. Vegans, gym zombies, hard-hats and spice fiends react differently to each. Skaters can only be fed by Slushie, Boba or Churro stations.
- **15 zombie types:** zombies are built from modular sprites in a 3/4 view, with random body shapes, genders, skin tones, hair and accessories. Body shape is purely cosmetic and never affects stats. Zombies bloat as they fill up and burst in a cartoon pop with no gore.
- **Field Guide:** an in-game book with every zombie, boss and station: stats, food preferences, per-tier tables and tips. Open it from the title screen or the pause menu.
- **Graveyard Shift:** an endless mode with every station available, open from the start.
- **Progression:** stars buy permanent Restaurant Upgrades, and gold buys in-run Secret Recipes. Everything is saved in localStorage.
- **Layout:** responsive landscape and portrait (the map is transposed on phones), with touch, mouse and optional keyboard controls. There is a reduced-motion option.
- **Art and sound:** all art is drawn in code, and all sound (zombie groans, pops, diner bell, surf-chiptune music) is synthesized with the Web Audio API.

## Controls
Pick a station, then tap a marked floor tile. On touch screens, tap once to preview and again to build. Tap a station to upgrade, sell or change its targeting.

Optional keys: `1-9, 0` stations · `R` recipes · `N` next wave · `F` speed · `Space` pause · `U` upgrade · `S` sell · `T` targeting · `Esc` cancel.

## Tweaking
All data lives at the top of the script: `STATIONS`, `ZOMBIES` (including food preferences), `THEMES`, `LEVELS` (paths and wave strings such as `"runner 8 0.6"`), `PERKS` and `RESEARCH`.
