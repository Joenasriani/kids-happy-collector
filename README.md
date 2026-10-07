# Happy Collector — 20-Level 3D Browser Platformer

![Happy Collector gameplay artwork from the official itch.io page](https://img.itch.zone/aW1nLzI3MzkyOTc3LnBuZw%3D%3D/original/49wel4.png)

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


---

## العربية

**Happy Collector** هي لعبة منصات ثلاثية الأبعاد تعمل في المتصفح باستخدام Three.js وتتكوّن من 20 مستوى. تم تطويرها كجزء من تجربة ترفيهية تعليمية تفاعلية متعددة الألعاب للأطفال في الإمارات العربية المتحدة.

تتحكم بمكعب أصفر مبتسم عبر مسارات من الجزر والمنصات العائمة. اجمع المكعبات الصفراء التي تحمل مشاعر وصفات إيجابية، وتجنب المكعبات الحمراء التي تمثل مشاعر وسلوكيات سلبية أو اقفز فوقها للتغلب عليها، ثم تجاوز تحديات المنصات والوصول إلى الباب المتوهج للانتقال إلى المستوى التالي.

**طريقة اللعب:** الحركة والقفز ← جمع المكعبات الإيجابية ← تجنب الأعداء السلبيين أو القفز فوقهم ← تجاوز العقبات ← الوصول إلى الباب المتوهج ← الانتقال للمستوى التالي.

- جمع مكعب أصفر: **+10 نقاط**
- القفز فوق عدو أحمر: **+5 نقاط**
- الاصطدام بعدو أحمر أو السقوط من المسار يفقدك محاولة
- تبدأ اللعبة بـ **3 محاولات**
- الوصول إلى الباب يكمل المستوى؛ جمع كل المكعبات الصفراء ليس شرطاً
- المستوى 20 هو المستوى الأخير

تتضمن اللعبة منصات أفقية متحركة، مصاعد عمودية، منصات بندولية، جسوراً منحنية وحبلية، بوابات تعمل بالأزرار، درجات ترتفع بالأزرار، منصات زجاجية تتشقق وتسقط بعد مغادرتها، وأعداء يقومون بدوريات ويمكن القفز فوقهم.

**التحكم على الكمبيوتر:** A/D أو الأسهم للحركة، وW أو Space أو السهم للأعلى للقفز، وعجلة الفأرة للتقريب والإبعاد أثناء اللعب.  
**على الهاتف:** أزرار الحركة والقفز على الشاشة، مع التكبير بإصبعين أثناء اللعب.


---

## Français

**Happy Collector** est un jeu de plateforme 3D en Three.js jouable dans le navigateur, composé de 20 niveaux. Il a été développé comme l'un des modules d'une activation interactive et ludo-éducative multi-jeux pour enfants aux Émirats arabes unis.

Vous contrôlez un cube jaune souriant à travers des parcours de plateformes flottantes. Collectez les blocs jaunes portant des émotions et qualités positives, évitez les blocs rouges représentant des émotions et comportements négatifs ou sautez dessus pour les éliminer, franchissez les obstacles et atteignez la porte lumineuse pour passer au niveau suivant.

**Boucle de jeu :** se déplacer et sauter → collecter les blocs positifs → éviter ou écraser les ennemis négatifs → franchir les obstacles → atteindre la porte lumineuse → avancer.

- Bloc jaune collecté : **+10 points**
- Ennemi rouge écrasé : **+5 points**
- Toucher un ennemi rouge ou tomber du parcours coûte une vie
- La partie commence avec **3 vies**
- Atteindre la porte termine le niveau ; collecter tous les blocs jaunes n'est pas obligatoire
- Le niveau 20 est le dernier niveau

Le jeu comprend des plateformes horizontales mobiles, des ascenseurs verticaux, des plateformes pendulaires, des ponts courbes et suspendus, des portes commandées par boutons, des marches relevables, des plateformes en verre qui se fissurent puis tombent après votre départ, et des ennemis en patrouille qui peuvent être écrasés.

**Ordinateur :** A/D ou flèches gauche/droite pour se déplacer ; W, Espace ou flèche haut pour sauter ; molette pour zoomer pendant le jeu.  
**Mobile :** commandes gauche/droite et saut à l'écran ; pincement à deux doigts pour zoomer pendant le jeu.


---

## 简体中文

**Happy Collector** 是一款使用 Three.js 制作、可直接在浏览器中游玩的 20 关 3D 平台游戏。它最初作为阿联酋儿童多游戏互动寓教于乐活动中的一个游戏模块开发。

玩家控制一个微笑的黄色方块，在漂浮的平台路线中前进。收集代表积极情绪与品质的黄色方块，避开代表消极情绪与行为的红色方块，或从上方踩掉它们；通过各种平台机关并到达发光的门，即可进入下一关。

**核心玩法：** 移动与跳跃 → 收集积极方块 → 避开或踩掉红色敌人 → 通过平台障碍 → 到达发光的门 → 进入下一关。

- 收集黄色方块：**+10 分**
- 从上方踩掉红色敌人：**+5 分**
- 碰到红色敌人或跌出路线会失去一次生命
- 每局开始时有 **3 条生命**
- 到达发光的门即可完成关卡；不需要收集全部黄色方块
- 第 20 关是最终关卡

游戏包含水平移动平台、垂直升降平台、摆动平台、弧形桥与绳桥、按钮控制的闸门、按钮升起的台阶、离开后会破裂坠落的玻璃平台，以及可被踩掉的巡逻敌人。

**电脑：** A/D 或左右方向键移动；W、空格键或上方向键跳跃；游戏中可使用鼠标滚轮缩放。  
**手机：** 使用屏幕上的左右移动与跳跃按钮；游戏中可双指缩放。



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
