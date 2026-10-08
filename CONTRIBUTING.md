# Contributing to Happy Collector

Happy Collector is a Three.js browser platformer with 20 existing levels. Contributions are welcome for level design, puzzle ideas, obstacle behavior, accessibility, performance, tests, and documentation.

You do not need to write code to suggest a level or puzzle. Start a GitHub issue with the concept and describe how the player would solve it.

## Ways to contribute

**Remix an existing level.** Suggest a different route, pacing, puzzle order, or obstacle combination. Keep the original level available. Do not replace an existing level without prior discussion.

**Design a puzzle.** Combine existing mechanics such as buttons, gates, lifts, moving platforms, pendulums, glass, and enemy patrols. Explain the solution and recovery path.

**Build a new level.** Propose a level after the existing 20. Level 21 is not implemented yet. Agree on the layout and mechanics before expanding the level count, HUD, progression, and completion logic.

**Improve the game.** Bug fixes, input reliability, performance, accessibility, and automated checks are welcome. Preserve existing behavior unless the change is specifically agreed upon.

## Start here

1. Play the [browser game](https://kids-happy-collector.vercel.app/).
2. Read the [level expansion guide](docs/HAPPY_COLLECTOR_LEVEL_EXPANSION_BIBLE.md) and [QA checklist](docs/PRE_DELIVERY_QA_CHECKLIST.md).
3. Search existing issues before proposing work.
4. Open an issue explaining the proposed change, its benefit, and which existing mechanics it uses.
5. Wait for scope agreement before making a large pull request.

## Working with the code

The game runs from `index.html`. It does not use a build system. For local testing, run `python3 -m http.server 8000` in the repository folder and open `http://localhost:8000/`.

The level generator starts at `generateLevelBlueprint(lvl)` in `index.html`. It uses helpers including `rest`, `gap`, `rise`, `descend`, `slider`, `lift`, `pendulum`, `curvedBridge`, `ropeBridge`, `gatePuzzle`, and `stairButtonPuzzle`. Level creation and runtime transitions also involve `spawnLevel` and `startLevelSequence`.

These are implementation functions, not a public level-editor API. A new level may require changes to progression and UI logic as well as the blueprint.

## Proposing a level or obstacle

Include:

- Proposed name and whether it is a remix, new level, or new mechanic
- A short sketch or description of the route
- What the player learns or has to work out
- The intended solution and any possible failure or recovery
- Existing primitives used and any code changes needed
- How the player reaches the door without unavoidable damage

Concept-only submissions are welcome. Screenshots or simple diagrams are enough for a first proposal.

## Pull requests

Keep each pull request focused on one change. Explain what changed and why. Include screenshots or a short gameplay recording for visual changes.

State exactly what was tested, including browser, device, and level range. Do not mark untested levels as passing. Follow the safety rules in the expansion guide: reachable exits, visible jumps, moving-platform clearance, fair enemy placement, and glass that does not collapse under the player.

Do not add third-party music, fonts, images, or code without documenting its source and redistribution license. The game's MIT license does not automatically cover third-party assets.

Accepted contributors will be credited in the relevant pull request and release notes. Contributions are reviewed for fit, playability, maintainability, and licensing; submission does not guarantee inclusion.
