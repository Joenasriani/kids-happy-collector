# Happy Collector : Pre-Delivery QA Checklist

Use this before sending any future ZIP/build.

## Package

- `index.html` exists at ZIP root.
- `/libs/three.r128.min.js` exists.
- `/music/` exists and contains the music files.
- `/sfx/` exists and contains SFX assets.
- ZIP integrity passes.
- No unrelated debug or build-export files are included in the gameplay ZIP.

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

## Contribution checks

For a level remix, new puzzle, or added level, record the affected level numbers, whether the original layouts remain accessible, the intended solution, and any failure or recovery cases. Check that no new obstacle causes unavoidable damage or blocks the exit.

For a new mechanic, also test at least one existing level using related systems to detect regressions.

## Verification record

The following is a record of what has been established from repository inspection. "Not recorded" does not mean a test failed; it means there is no documented test result.

| Check | Status | Evidence |
| --- | --- | --- |
| Local Three.js file present | Confirmed in repository | `libs/three.r128.min.js` |
| Font files present | Confirmed in repository | `fonts/` |
| Music and wind audio files present | Confirmed in repository | `music/`, `sfx/` |
| Desktop browser playthrough, levels 1 to 20 | Not recorded | No complete run log |
| Mobile portrait and landscape playthrough | Not recorded | No device test log |
| Cross-browser WebGL compatibility | Not recorded | No browser matrix |
| All levels reachable and passable | Not recorded | No complete playthrough results |
| JavaScript syntax validation on current commit | Not recorded | No test result attached |

For each future test, record the commit, date, browser/version, device, level(s), steps, result and any issue link. Keep source inspection separate from runtime verification.
