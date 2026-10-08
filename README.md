# Happy Collector: 20-Level Three.js Browser Platformer

<p align="center">
  <img src="assets/readme/happy-collector-banner.png" alt="Happy Collector" width="100%">
</p>

<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.ar.md">العربية</a> ·
  <a href="README.fr.md">Français</a> ·
  <a href="README.zh-CN.md">简体中文</a>
</p>

**Play:** https://kids-happy-collector.vercel.app/  
**Itch.io:** https://joenasr.itch.io/happy-collector

Happy Collector is a 20-level Three.js browser platformer developed as one module in a multi-game interactive children's edutainment activation in the UAE.

You control a smiling yellow cube along floating platform routes. Yellow blocks carry positive emotions and qualities; red moving enemies carry negative emotions and behaviors. Collect yellow blocks for points, avoid or stomp red enemies, navigate platform obstacles, and reach the level door to advance.

## For developers and level designers

Happy Collector is a playable Three.js and WebGL platformer built with JavaScript in one `index.html` file. It uses reusable level blueprints, custom movement and collision logic, patrolling enemies, moving platforms, glass platforms, and button-operated puzzles. No build system is required to inspect or run it.

Want to experiment with the level design? You can [remix an existing level](https://github.com/Joenasriani/kids-happy-collector/issues/7), [design a new puzzle](https://github.com/Joenasriani/kids-happy-collector/issues/8), or [propose an obstacle](https://github.com/Joenasriani/kids-happy-collector/issues/9). JavaScript developers can also help [validate level reachability](https://github.com/Joenasriani/kids-happy-collector/issues/10). Concepts and sketches are welcome before code. See [CONTRIBUTING.md](CONTRIBUTING.md).

## How it plays

**move and jump → collect positive blocks → avoid or stomp red enemies → navigate obstacles → reach the door → advance**

- Yellow collectible: **+10 points**
- Stomp a red enemy from above while descending: **+5 points**
- Contact with a red enemy or falling from the route costs one life
- You start a run with **3 lives**
- After losing a life, the current level restarts while the remaining lives persist
- Collecting every yellow block is **not required** to finish a level
- Reaching the door advances to the next level
- Completing Level 20 ends the run with **MASTER COLLECTOR!**

Yellow blocks use the labels **BRAVERY, JOY, LOVE, HOPE, PEACE, KINDNESS, CALM, PRIDE, TRUST, HAPPINESS**. Red-enemy labels are **ANGER, GREED, JEALOUSY, RUDENESS, ENVY, HATE, DESPAIR**.

## Controls

**Desktop**
- `A / D` or `Left / Right Arrow` : move
- `W`, `Space`, or `Up Arrow` : jump
- Mouse wheel : zoom after gameplay movement begins

**Mobile**
- On-screen left/right controls : move
- On-screen jump control : jump
- Two-finger pinch : zoom after gameplay movement begins

## Gameplay systems

The game includes horizontal and vertical moving platforms, pendulum platforms, curved and rope-bridge sequences, button-controlled gates, button-raised steps, cracking glass platforms, stompable patrolling enemies, changing skies, ambient scenery, level-introduction cinematics, door-arrival transitions, six looping music tracks, synthesized gameplay SFX, cinematic wind audio, visual feedback and supported-device vibration.

Glass platforms crack when stood on, remain solid while occupied, then fall and fade after the player leaves. Legacy pop-up/falling path-platform behavior is disabled.

## Level architecture

The game builds all 20 levels from reusable platform and obstacle definitions. Levels 11 to 20 use these named layouts:

11. Glass Garden Switchback  
12. Cracking Orchard Bridge  
13. Button Garden Run  
14. Pendulum Picnic Crossing  
15. Raised Stair Workshop  
16. Bad Habit Patrol Park  
17. Cloud Lift Labyrinth  
18. Glass Habit Trial  
19. Switchback Sky Garden  
20. Good Habit Summit

## Implementation

- `index.html` : complete playable game and runtime logic
- `libs/three.r128.min.js` : local Three.js r128 runtime
- `libs/THREE_LICENSE.txt` : bundled Three.js license
- `music/` : six local music tracks
- `sfx/` : local cinematic wind audio
- `fonts/` : local fonts
- `docs/` : level-expansion rules and pre-delivery QA documentation

Three.js loads from the local `libs/` folder. Most gameplay sound effects are generated with the Web Audio API.

## Code navigation

The game lives in `index.html`. Search for these functions to find the relevant systems:

| Function | Purpose |
| --- | --- |
| `generateLevelBlueprint(lvl)` | Builds reusable platform and obstacle layouts |
| `getLevelBlueprint(lvl)` | Retrieves the level blueprint |
| `spawnLevel` | Creates a level's playable scene |
| `startLevelSequence` | Starts level progression and introduction |
| `createTextCanvas` | Draws words on collectible and enemy textures |

See the [level expansion guide](docs/HAPPY_COLLECTOR_LEVEL_EXPANSION_BIBLE.md) for gameplay constraints. The functions are internal implementation details, not a public level editor.

## Run locally

Download or clone this repository. Keep `index.html`, `libs/`, `fonts/`, `music/`, and `sfx/` together.

From the repository folder, start a local HTTP server:

```sh
python3 -m http.server 8000
```

Open `http://localhost:8000/` in a browser with WebGL support. Python 3 is needed only for this local server, not for the game. No package installation or build step is required. Avoid opening `index.html` directly as a `file://` URL because browser asset-loading restrictions may interfere with local files.

## Contributing

Want to build a different puzzle, remix a level, or extend the game beyond Level 20? Ideas from level designers and developers are welcome.

Start with [CONTRIBUTING.md](CONTRIBUTING.md). It explains how to propose a level, work with the existing blueprint functions, and submit changes. The original 20 levels stay available while alternate layouts and new mechanics are reviewed separately.

## Testing status

The repository includes a [pre-delivery QA checklist](docs/PRE_DELIVERY_QA_CHECKLIST.md), but that checklist is not proof of completed testing. A full browser playthrough of all 20 levels, device-specific mobile checks, and cross-browser regression results have not been recorded in this repository.

For future changes, record the browser and device tested, the level range, the checks performed, and any failures. Do not mark a check as passed without running it.

## Event activation

Happy Collector was developed as one module in a multi-game interactive children's edutainment activation in the UAE.

Event production: [Peach Society](https://peach-society.com/), Dubai.

## Audio credits

Music by **BombinSound** and **AleXZavesa**. Wind sound effect by **DRAGON-STUDIO**. The seven audio files are linked to their original Pixabay listings in [AUDIO_CREDITS.md](AUDIO_CREDITS.md). Pixabay's media license is separate from the game's MIT source-code license.

## Licensing

Original Happy Collector source code and documentation are released under the [MIT License](LICENSE). Third-party libraries, fonts, music, sound effects, artwork and branding are not relicensed by MIT. See [third-party asset rights](THIRD_PARTY_ASSETS.md) before redistributing the complete game.

The bundled Three.js license is in `libs/THREE_LICENSE.txt`. Font licenses are in `fonts/`. Audio source pages and Pixabay licensing terms are documented in [AUDIO_CREDITS.md](AUDIO_CREDITS.md). Artwork rights should be checked separately.
