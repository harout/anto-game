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

## ✎ Level editor
Open **＋ LEVEL EDITOR** in the track menu to build your own track from sections — straights, turns, climbs and drops,
canyons with arches, tunnels, rivers (slow you down) or swamp water (full speed), ramp jumps and rock fields — in any of the
five worlds, with 1–9 laps. A live map and height profile show the track as you build it. Your levels appear as cards in
the menu and race with the AI rivals, ghosts and standings like the built-in tracks. **🎢 BUILD IN 3D** lets you build Planet Coaster-style: pick the next piece's length, turn (22°/45°/90°), slope and type,
see it glow at the end of the track in 3D, and press Enter to place it (Backspace to undo).
**🧪 TEST DRIVE** drives the level right away without saving (one lap, no rivals; Esc returns to the editor).
**≈✕ Remove water** clears every river and swamp stretch at once.
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
