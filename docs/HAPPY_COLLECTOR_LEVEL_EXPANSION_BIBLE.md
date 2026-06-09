# Happy Collector - Future Level Expansion Bible

Last updated: 2026-06-09

## Current release baseline

Use `Happy_Collector_Clean_Self_Contained_Release.zip` as the source for future work.

The game is a cheerful single-file Three.js browser platformer. The player controls a smiling yellow cube across floating green island platforms, collects yellow Good Habit blocks, avoids or stomps red Bad Habit blocks, solves simple platform obstacles, rides moving platforms, and reaches a glowing generated door.

## Locked systems - do not change unless explicitly requested

- player physics
- movement speed
- jump feel
- desktop controls
- mobile controls
- camera behavior
- UI layout direction
- start page
- music system
- SFX system
- score system
- generated glowing door
- green floating island visual style
- yellow smiling cube character
- no-arm character state
- fall SFX threshold rule
- explosion and Try Again timing
- door transition timing
- secret LEVELS menu behavior, unless intentionally preparing a public-only build

## Core controls

- move left
- move right
- jump

Do not add dash, double jump, climbing, weapons, inventory, Z-axis walking, free 3D movement, rotating gameplay camera, or spiral/tower gameplay.

## Permanent gameplay rules

1. Falling SFX triggers only after the character falls below the lowest platform threshold.
2. Falling SFX must not trigger during level start drop, normal descent, jumps to lower blocks, or ordinary falling arcs before the threshold.
3. Explosion and Try Again timing remain unchanged.
4. Dynamic moving blocks must never merge into, go into, or visually touch other blocks.
5. Moving platforms must maintain a visible safety gap through the full motion path.
6. Dynamic platforms must be structural and gameplay-relevant, never decorative only.
7. Every obstacle must be mathematically solvable.
8. No impossible jumps.
9. No blind jumps.
10. No unavoidable damage.
11. Every level must have a distinct identity and silhouette.
12. Difficulty increases gradually.
13. The door must be reachable and sit on a valid platform/floor surface.
14. Do not use ordinary falling/drop-style dynamic path bricks.
15. Do not use sudden random drop blocks.
16. Do not use the spiral/tower level idea unless explicitly requested again.

## Approved obstacle/block types

- static green island platforms
- slider bridge / horizontal moving block
- up/down elevator platform
- button opens gate
- button-raised stair step
- pendulum platform
- rope bridge sections
- curved wooden bridge / curved wooden bridge run
- enemy patrol corridor
- enemy guarded exit
- glass brick

## Glass brick rule

Glass bricks are allowed only as a special mechanic.

Behavior:

1. Player lands on glass brick.
2. That exact brick cracks and plays crack SFX.
3. Brick remains solid while the player stands on it.
4. When the player jumps/leaves, that exact brick falls and fades away.

Rules:

- only the touched glass brick cracks
- no path-wide cracking animation
- ordinary green path bricks never crack/fall
- glass must not fall while player is standing on it
- next jump must be possible and visible
- do not overuse glass as stress spam

## Enemy patrol rule

Enemies are red Bad Habit blocks.

Rules:

- no enemies on blind landings
- no forced damage
- no enemy directly camping the door platform
- no enemies on tiny unfair platforms
- short patrol ranges use slow patrol mode and edge pauses
- wide patrol corridors may use normal patrol speed
- every enemy corridor needs a safe approach zone and enough room to jump or stomp

## Authored level direction

Levels 11-20 were rebuilt with authored identities:

- Level 11 - Glass Garden Switchback
- Level 12 - Cracking Orchard Bridge
- Level 13 - Button Garden Run
- Level 14 - Pendulum Picnic Crossing
- Level 15 - Raised Stair Workshop
- Level 16 - Bad Habit Patrol Park
- Level 17 - Cloud Lift Labyrinth
- Level 18 - Glass Habit Trial
- Level 19 - Switchback Sky Garden
- Level 20 - Good Habit Summit

Future levels should follow the same pattern:

- one clear silhouette
- one gameplay idea
- one readable aha moment
- optional reward route, not mandatory punishment
- safe final landing before the glowing door
- no filler chains added only to increase length

## Future level creation workflow

For each new level:

1. Define the level title.
2. Define the visual silhouette.
3. Define the one core mechanic idea.
4. Build only that level.
5. Audit geometry and passability.
6. Check dynamic-platform clearances.
7. Check glass self-only behavior if glass is used.
8. Check enemy fairness if enemies are used.
9. Run JavaScript syntax check.
10. Check ZIP integrity and root `index.html`.
11. Report honestly what was verified and what was not.

Do not bulk build multiple levels without auditing each one.
