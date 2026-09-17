# Happy Collector — Good Habits Adventure

Play: https://kids-happy-collector.vercel.app/

Itch.io: https://joenasr.itch.io/happy-collector

Happy Collector is a 20-level 3D browser platformer developed as part of a multi-game interactive children’s edutainment activation in the UAE. The player controls a yellow cube across floating platforms, collects yellow **Good Habit** blocks, avoids or stomps red **Bad Habit** blocks, uses moving platforms, crosses cracking glass sections, and reaches the level exit.

## Game structure

**platform movement → collect Good Habit blocks → avoid or stomp Bad Habit blocks → navigate level obstacles → reach the exit → advance to the next level**

The current game implements 20 levels. Levels 11–20 have authored level identities, and Level 20 is the final level.

## Controls

### Desktop

- `A / D` or `Left / Right Arrow` — move
- `Space` or `Up Arrow` — jump

### Mobile

- on-screen left/right controls — move
- on-screen jump control — jump

## Activation context

This game belongs to the same `kids-*` game set developed for the multi-game interactive children’s edutainment activation in the UAE.

## Repository structure

- `index.html` — playable game
- `libs/` — local Three.js runtime and license
- `music/` — music assets
- `sfx/` — sound-effect assets
- `fonts/` — local font assets
- `docs/` — level-expansion and pre-delivery QA documentation

The playable game is intentionally preserved. Public-context and discovery files must not change game logic, controls, scoring, progression, levels, timing, assets, visual behavior, audio behavior, or runtime behavior.
