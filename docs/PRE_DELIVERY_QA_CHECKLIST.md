# Happy Collector - Pre-Delivery QA Checklist

Use this before sending any future ZIP/build.

## Package

- `index.html` exists at ZIP root.
- `/libs/three.r128.min.js` exists.
- `/music/` exists and contains the music files.
- `/sfx/` exists and contains SFX assets.
- ZIP integrity passes.
- No unrelated audit JSON/page-kit/debug exports are included in the gameplay ZIP.

## External dependencies

- Three.js uses `./libs/three.r128.min.js`, not CDN.
- No critical runtime script depends on network access.
- External fonts are optional only; the game must remain usable without them.

## Code safety

- JavaScript syntax check passes.
- Search for `.clear()` and confirm none run before declarations.
- Search for `= []` and confirm array resets happen only after declaration and inside lifecycle functions.
- Search for `= new Map()` and confirm no cleanup/reset happens before initialization.
- No accidental duplicate input handlers.
- No broken level references.

## Gameplay invariants

- Player physics unchanged.
- Movement speed unchanged.
- Jump feel unchanged.
- Camera unchanged.
- Desktop controls unchanged.
- Mobile controls unchanged.
- UI layout direction unchanged.
- Music/SFX systems unchanged.
- Fall SFX threshold unchanged.
- Explosion and Try Again timing unchanged.
- Door transition timing unchanged.

## Level safety

- Door is reachable and sits on a valid surface.
- No impossible jumps.
- No blind jumps.
- No unavoidable damage.
- Moving platforms never touch/merge with static platforms.
- Dynamic platforms keep visible safety gaps.
- Glass only affects the exact touched glass brick.
- Ordinary green path bricks never fall.
- Short enemy patrol platforms use slow patrol behavior.
- Secret LEVELS menu still opens only through the hidden code.

## Truthfulness rule

Never claim live browser/mobile/WebGL playthrough unless it was actually performed.
