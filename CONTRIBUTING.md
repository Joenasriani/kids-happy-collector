# Contributing to Happy Collector

Happy Collector is a Three.js browser platformer with 20 existing levels. Any idea is welcome if it can produce a real improvement, experiment, feature, design, tool, performance gain, accessibility gain, or useful extension.

The current game is the starting point, not the ceiling. Contributors may explore new mechanics, level systems, visuals, tools, interfaces, and different approaches. The examples below are entry points, not limits.

You can propose a concept, sketch, prototype, code change, or experiment. Explain what it aims to improve and how its value could be evaluated. Larger or riskier changes can be developed separately and reviewed before integration.

## Open challenges

- [Remix an existing level](https://github.com/Joenasriani/kids-happy-collector/issues/7)
- [Design a button and gate puzzle](https://github.com/Joenasriani/kids-happy-collector/issues/8)
- [Propose a new obstacle](https://github.com/Joenasriani/kids-happy-collector/issues/9)
- [Build a level-reachability check](https://github.com/Joenasriani/kids-happy-collector/issues/10)

You can submit a design concept before writing code.

## Examples of contributions

**Remix or redesign levels.** Suggest different routes, pacing, puzzles, or obstacle combinations. Changes to existing levels can be proposed and evaluated against the current version.

**Design a puzzle.** Combine existing mechanics such as buttons, gates, lifts, moving platforms, pendulums, glass, and enemy patrols. Explain the solution and recovery path.

**Extend the game.** Propose additional levels, new level structures, modes, mechanics, or tools. Level 21 is not implemented yet. Larger changes may also require updates to progression, HUD, and completion logic.

**Improve or experiment.** Explore performance, accessibility, controls, rendering, visual design, gameplay systems, automated checks, developer tools, and other ideas. Explain the benefit and any effect on current behavior.

## Start here

1. Play the [browser game](https://kids-happy-collector.vercel.app/).
2. Read the [level expansion guide](docs/HAPPY_COLLECTOR_LEVEL_EXPANSION_BIBLE.md) and [QA checklist](docs/PRE_DELIVERY_QA_CHECKLIST.md).
3. Search existing issues before proposing work.
4. Open an issue explaining the proposed change, expected benefit, and any systems it may affect.
5. Wait for scope agreement before making a large pull request.

## Working with the code

The game runs from `index.html`. It does not use a build system. For local testing, run `python3 -m http.server 8000` in the repository folder and open `http://localhost:8000/`.

The level generator starts at `generateLevelBlueprint(lvl)` in `index.html`. It uses helpers including `rest`, `gap`, `rise`, `descend`, `slider`, `lift`, `pendulum`, `curvedBridge`, `ropeBridge`, `gatePuzzle`, and `stairButtonPuzzle`. Level creation and runtime transitions also involve `spawnLevel` and `startLevelSequence`.

These are implementation functions, not a public level-editor API. A new level may require changes to progression and UI logic as well as the blueprint.

## Proposing an idea

Include what applies:

- What you want to improve, create, or test
- The expected benefit or question the experiment will answer
- A sketch, prototype, example, or technical approach where useful
- Which existing systems may change
- How the result could be evaluated
- Any known compatibility, gameplay, accessibility, or licensing concerns

Concept-only submissions are welcome. Screenshots or simple diagrams are enough for a first proposal.

## Pull requests

Keep each pull request focused on one change. Explain what changed and why. Include screenshots or a short gameplay recording for visual changes.

State exactly what was tested, including browser, device, and level range. Do not mark untested levels as passing. For gameplay changes, check the relevant safety rules in the expansion guide, including reachable exits, readable jumps, moving-platform clearance, fair enemy placement, and recoverable failure states. Experimental designs can depart from existing mechanics when the change is intentional and tested.

Do not add third-party music, fonts, images, or code without documenting its source and redistribution license. The game's MIT license does not automatically cover third-party assets.

Accepted contributors will be credited in the relevant pull request and release notes. Contributions are reviewed for fit, playability, maintainability, and licensing; submission does not guarantee inclusion.
