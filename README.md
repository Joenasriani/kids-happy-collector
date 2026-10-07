# Happy Collector — 20-Level 3D Browser Platformer

**Play:** https://kids-happy-collector.vercel.app/  
**Itch.io:** https://joenasr.itch.io/happy-collector

Happy Collector is a 20-level Three.js browser platformer developed as part of a multi-game interactive children's edutainment activation in the UAE.

You control a smiling yellow cube across floating island routes. Collect yellow blocks carrying positive emotions and qualities, avoid or stomp red blocks carrying negative emotions and behaviors, navigate increasingly complex platform challenges, and reach the glowing door to advance.

## How it plays

**move and jump → collect positive blocks → avoid or stomp negative blocks → navigate obstacles → reach the glowing door → advance**

Collectibles are optional for progression: reaching the door completes the level.

- Yellow collectible: **+10 points**
- Stomp a red enemy from above: **+5 points**
- Contact with a red enemy or falling from the route costs a life
- You begin with **3 lives** for the run
- Level 20 is the final level

The block labels are drawn from the game's runtime data. Positive examples include **BRAVERY, JOY, LOVE, HOPE, PEACE, KINDNESS, CALM, PRIDE, TRUST, HAPPINESS**. Negative examples include **ANGER, GREED, JEALOUSY, RUDENESS, ENVY, HATE, DESPAIR**.

## Controls

### Desktop

- `A / D` or `Left / Right Arrow` — move
- `W`, `Space`, or `Up Arrow` — jump
- Mouse wheel — zoom after gameplay movement begins

### Mobile

- On-screen left/right controls — move
- On-screen jump control — jump
- Two-finger pinch — zoom after gameplay movement begins

## Gameplay systems

The game includes:

- horizontal moving platforms
- vertical lifts
- pendulum platforms
- curved and rope-bridge sequences
- button-controlled gates
- button-raised steps
- cracking glass platforms that fall after the player leaves them
- patrolling red enemies that can be stomped
- changing sky environments, clouds and ambient scenery
- level-introduction cinematics and a glowing-door transition
- music, synthesized sound effects, feedback particles and supported-device haptics

## Level architecture

The game uses a deterministic blueprint-generation system rather than 20 isolated static maps. Levels are assembled from reusable platform and obstacle primitives.

Levels 11–20 have explicitly authored high-level sequences:

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

Legacy pop-up/falling path bricks are disabled in the current runtime.

## Languages

The game includes an in-game language switcher for:

- English
- Arabic (RTL)
- French
- Simplified Chinese

Localization covers the start instructions, HUD labels, level/game-over messaging, gameplay feedback, and the words rendered on positive collectibles and negative enemies.

## Implementation

- `index.html` — complete playable game and runtime logic
- `libs/three.r128.min.js` — local Three.js runtime
- `libs/THREE_LICENSE.txt` — Three.js license
- `music/` — music assets
- `sfx/` — sound-effect assets
- `fonts/` — local fonts
- `docs/` — level-expansion rules and pre-delivery QA documentation

The playable runtime does not depend on a CDN for Three.js.

## Event activation

Happy Collector was developed as one module in a multi-game interactive children's edutainment activation in the UAE.

Event production: [Peach Society](https://peach-society.com/) — Dubai-based event and experiential production company.

## Licensing

The repository currently does **not** declare a project-wide license. The bundled Three.js license applies to Three.js; it should not be interpreted as automatically licensing the Happy Collector game code, artwork, audio, fonts, or other project assets.
