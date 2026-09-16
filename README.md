# Happy Collector - Good Habits Adventure

A cheerful 3D HTML5 browser platformer where a smiling yellow cube collects **Good Habit** blocks, avoids or stomps red **Bad Habit** blocks, rides floating island platforms, survives cracking glass bricks, and reaches the glowing door.

## Current release status

This repository should track the final browser release candidate prepared for itch.io.

Current intended build features:

- 20 playable levels
- Authored Levels 11-20
- Local/self-contained Three.js build
- No external CDN dependency
- No Google Fonts dependency
- Music and SFX folders preserved
- Glass crack SFX
- Visual/audio feedback polish
- Short-platform patrol slowdown
- Hidden developer level menu for testing
- Future-useful docs in `docs/`

## Controls

### Desktop

- `A / D` or `Left / Right Arrow` - Move
- `Space` or `Up Arrow` - Jump

### Mobile

- Use the on-screen left/right buttons
- Tap the jump button

## Included assets

- `index.html` - main game file
- `libs/` - local Three.js and license
- `music/` - level music tracks
- `sfx/` - cinematic wind / sound effects
- `fonts/` - optional local font placement
- `docs/` - continuation and QA rules for future levels

## Important release note

The final itch.io-ready ZIP generated in ChatGPT is the source of truth for public upload:

`Happy_Collector_ItchIO_Final_Upload.zip`

If this repository is missing `libs/three.r128.min.js`, upload the ZIP contents manually into the repo root before deploying from GitHub Pages.

## Credits

- Game Dev: ApexInnovate.ae
- Music: BombInSound, AlexZavesa
