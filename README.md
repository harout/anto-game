# anto-game — Podracer

A pseudo-3D pod racing game that runs in the browser and is built to be flown with a
**Thrustmaster HOTAS Warthog throttle** (left and right levers drive the left and right engines).

**Play:** https://harout.github.io/anto-game/

## How to play
- Open the page in **Chrome** (Safari can't see HOTAS controllers).
- Move a throttle lever or press a button on the Warthog so Chrome wakes the controller up,
  then use **Map throttles** in the controller panel to calibrate. Calibration is saved in the browser.
- Push both levers to go faster; split them to steer.

| Control | Warthog | Keyboard |
|---|---|---|
| Throttle / steer | left + right levers | W / S both, Q / A left, E / D right, ← → steer |
| Boost | button 14 | Space |
| Super boost | button 13 | L |
| Laser (tap) / homing missile (hold) | button 0 | F |
| Shield | button 23 | G |

## Tracks
- **Dune Cup** — desert canyons, a cave and slot-canyon shortcuts with chasm jumps
- **Frost Canyon** — ice world (unlocked by your first win)
- **Forest Run** — one long lap climbing through 15 caves to an Everest-high summit, with forks, secret paths and frozen rivers
- **Swamp Run** — dead flat; skim across the swamp water at full speed
- **Bryce Canyon** — a rim road above a hoodoo amphitheater, switchbacks down through the hoodoos, and the Wall Street slot-canyon shortcut
- **🌌 Grand Tour** — all five worlds in one race. Between worlds your pod lifts off and flies at the speed of light:
  steer with the throttles, push both levers up to climb, fly through rings to save time and dodge space rocks

Seven AI rivals race you. Each 1st place on a track makes that track's rivals 1% smarter —
up to an exact copy of you and your pod — and at level 50 they learn that track's shortcuts.

## 🎨 Paint shop
**🎨 CUSTOMIZE POD** in the menu: paint color, engine finish (light, dark, chrome, gold, white), pattern (stripes, flames,
checkers, race number), engine glow, energy beam and helmet colors, and a nickname for the standings — saved per pod,
cosmetic only. The pod revs behind the panel as a live preview (🔥 TRY BOOST shows the boost flames).

## ✎ Level editor
Open **＋ LEVEL EDITOR** in the track menu to build your own track from sections — straights, turns, climbs and drops,
canyons with arches, tunnels, rivers (slow you down) or swamp water (full speed), ramp jumps and rock fields — in any of the
five worlds, with 1–9 laps. A live map and height profile show the track as you build it. Your levels appear as cards in
the menu and race with the AI rivals, ghosts and standings like the built-in tracks. **🎢 BUILD IN 3D** lets you build Planet Coaster-style: pick the next piece's length, turn (22°/45°/90°), slope and type,
see it glow at the end of the track in 3D, and press Enter to place it (Backspace to undo).
**🧪 TEST DRIVE** drives the level right away without saving (one lap, no rivals; Esc returns to the editor).
**≈✕ Remove water** clears every river and swamp stretch at once; **⤴✕ Remove ramps** clears every ramp jump.
**✕ Overpasses**: where your track crosses itself, the lower road goes through a tunnel and the upper one becomes a bridge
(lifted if needed); from the bridge you can see the lower road crossing underneath.
**🔄 Auto-complete** adds the turn, straight and turn that join the end of your track back to the start line, level with it.
**⑂ Split tracks**: any plain section can split off a second route (left or right — a side road, log jumps, a creek,
a rock tunnel or a boulder garden) that rejoins at the end of the section; rivals take it now and then.
**⧉ SHARE CODE** gives a code
(starting with `POD1:`) a friend can paste into **⇩ IMPORT CODE**.

**AI smartness** — a slider in the menu sets the rivals' level yourself on each track (0–50; at 50 they know the shortcuts).

**Beat the Grand Tour in 1st place** to unlock:
- **👻 Ghost race** — no rivals, just you against a see-through replay of your own best run on that track,
  with a live “ahead / behind your best” readout. Beat it and your new run becomes the ghost.

Everything is in a single self-contained `index.html` — no build step, no dependencies.

## 🔧 Garage & pod upgrades
Every race pays credits (300 for 1st down to 90 for 8th, plus about 1 per 2 seconds raced; the Grand Tour pays double, ghost races 60). Spend them in the **🔧 GARAGE** on the menu. Each pod has its own upgrades, 5 levels each: Engine (top speed), Thrusters (acceleration), Steering, Boost power, Boost tank (boost lasts longer) and Armor (keep more speed when you crash). Level costs 100, 200, 300, 400, 500. You can sell all of a pod's upgrades for a full refund. The green part of the stat bars shows your upgrades.

## 🔐 Secret levels
Ten secret levels are hidden behind **secret missions** all over the game: hacks, hidden menus, cheat codes, hyperspace voices and more. Open **🔐 SECRET LEVELS** on the menu to read the clue for each mission (press 💡 if you're stuck). Finish a mission and a 📡 SECRET TRANSMISSION gives you a code. Type the code to open that level. Codes work on any computer. The final mission only works once the other 9 secret levels are open. No spoilers here!

## ✎ Ten new editor pieces
- **🕳 Canyon jump**: a ramp and a gap in the canyon floor. Hold BOOST or you fall in and restart at the run-up.
- **⛰ Wall notch + rim**: a notch in a canyon wall leads up onto the rim, across a canyon jump and back down.
- **🎢 Loop-the-loop**: a roller-coaster loop made of solid rock, like a natural stone arch bent into a circle (red sandstone, icy rock, granite or mossy stone depending on the world). You can see the track curl up into a giant circle as you drive towards it. On the ride the camera follows the track up, upside down over the top (ground overhead, sky below) and back down. A loop where the track crosses over itself turns into plain road.
- **⚡ Speed pads**: green arrows that fling you forward.
- **🔋 Refill pads**: blue pads that fill your boost tank.
- **〰 Whoops**: a row of bumps.
- **🧊 Ice**: a sheet of ice with no grip.
- **🪨 Bumpy road**: rough, rocky ground that slows you a little.
- **↔ Narrow road**: half the width, so stay on it.
- **🌪 Sandstorm**: thick haze (a blizzard on ice, mist in the swamp and forest) and gusts that push you sideways.

Also fixed: AI pods on the main track never refilled their boost after using it.

## 💾 Save & exit
The level editor has a green **💾 SAVE & EXIT** button at the top and at the bottom. It saves your level and takes you back to the menu.

## ✎ Lots of your own levels
The **＋ NEW LEVEL** card on the menu always starts a brand-new level. Each level you've made has its own card with **✎ EDIT** (change it) and **🗑** (delete it, click twice).
