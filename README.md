# Happy Collector — 20-Level Three.js Browser Platformer

<p align="center">
  <img src="assets/readme/file_000000007a1072469e9f473974c71db0-2.png" alt="Happy Collector" width="100%">
</p>


**Play:** https://kids-happy-collector.vercel.app/  
**Itch.io:** https://joenasr.itch.io/happy-collector

## English

Happy Collector is a 20-level Three.js browser platformer developed as one module in a multi-game interactive children's edutainment activation in the UAE.

You control a smiling yellow cube along floating platform routes. Yellow blocks carry positive emotions and qualities; red moving enemies carry negative emotions and behaviors. Collect yellow blocks for points, avoid or stomp red enemies, navigate platform obstacles, and reach the level door to advance.

### How it plays

**move and jump → collect positive blocks → avoid or stomp red enemies → navigate obstacles → reach the door → advance**

- Yellow collectible: **+10 points**
- Stomp a red enemy from above while descending: **+5 points**
- Contact with a red enemy or falling from the route costs one life
- You start a run with **3 lives**
- After losing a life, the current level restarts while the remaining lives persist
- Collecting every yellow block is **not required** to finish a level
- Reaching the door advances to the next level
- Completing Level 20 ends the run with **MASTER COLLECTOR!**

The runtime's yellow-block labels are **BRAVERY, JOY, LOVE, HOPE, PEACE, KINDNESS, CALM, PRIDE, TRUST, HAPPINESS**. Red-enemy labels are **ANGER, GREED, JEALOUSY, RUDENESS, ENVY, HATE, DESPAIR**.

### Controls

**Desktop**

- `A / D` or `Left / Right Arrow` — move
- `W`, `Space`, or `Up Arrow` — jump
- Mouse wheel — zoom after gameplay movement begins

**Mobile**

- On-screen left/right controls — move
- On-screen jump control — jump
- Two-finger pinch — zoom after gameplay movement begins

### Gameplay systems

The current runtime includes:

- horizontal moving platforms
- vertical moving platforms/lifts
- pendulum platforms
- curved bridge and rope-bridge platform sequences
- button-controlled gates
- button-raised steps
- glass platforms that crack when stood on, remain solid while occupied, then fall and fade after the player leaves
- patrolling red enemies that can be stomped
- different sky treatments, including night levels with stars
- clouds and ambient decorative scenery
- level-introduction cinematics
- door-arrival transitions
- six looping music tracks selected by level
- synthesized gameplay sound effects plus a separate cinematic wind audio asset
- visual feedback effects and vibration on supported devices

Legacy pop-up/falling path-platform behavior is disabled in the current runtime.

### Level architecture

All 20 levels are produced by the runtime's deterministic blueprint generator from reusable platform and obstacle primitives. Levels 11–20 contain explicitly authored high-level sequences:

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

---

## العربية

**Happy Collector** هي لعبة منصات ثلاثية الأبعاد من 20 مستوى تعمل في المتصفح باستخدام Three.js. تم تطويرها كوحدة ضمن تجربة تفاعلية تعليمية ترفيهية متعددة الألعاب للأطفال في الإمارات العربية المتحدة.

تتحكم بمكعب أصفر مبتسم على مسارات من المنصات العائمة. تحمل المكعبات الصفراء مشاعر وصفات إيجابية، بينما يحمل الأعداء الحمر المتحركون مشاعر وسلوكيات سلبية. اجمع المكعبات الصفراء للنقاط، وتجنب الأعداء الحمر أو اقفز فوقهم من الأعلى، وتجاوز العقبات، ثم صِل إلى باب المستوى للانتقال إلى المستوى التالي.

- المكعب الأصفر: **+10 نقاط**
- القضاء على عدو أحمر بالقفز عليه من الأعلى أثناء الهبوط: **+5 نقاط**
- الاصطدام بعدو أحمر أو السقوط من المسار يفقدك حياة واحدة
- تبدأ الجولة بـ **3 حيوات**
- بعد خسارة حياة، يُعاد المستوى الحالي مع الاحتفاظ بعدد الحيوات المتبقية
- جمع جميع المكعبات الصفراء **ليس شرطاً** لإنهاء المستوى
- الوصول إلى الباب ينقلك إلى المستوى التالي
- إنهاء المستوى 20 ينهي الجولة برسالة **MASTER COLLECTOR!**

الكلمات الموجودة على المكعبات الصفراء في اللعبة هي: **BRAVERY, JOY, LOVE, HOPE, PEACE, KINDNESS, CALM, PRIDE, TRUST, HAPPINESS**. أما الأعداء الحمر فهم: **ANGER, GREED, JEALOUSY, RUDENESS, ENVY, HATE, DESPAIR**.

**التحكم على الكمبيوتر:** `A / D` أو الأسهم يمين/يسار للحركة؛ `W` أو `Space` أو السهم للأعلى للقفز؛ عجلة الفأرة للتقريب والإبعاد بعد بدء الحركة.  
**على الهاتف:** أزرار الحركة والقفز على الشاشة؛ والتكبير بإصبعين بعد بدء الحركة.

تشمل اللعبة منصات أفقية وعمودية متحركة، منصات بندولية، مسارات جسور منحنية وحبلية، بوابات تعمل بالأزرار، درجات ترتفع بالأزرار، منصات زجاجية تتشقق عند الوقوف عليها وتبقى صلبة أثناء الوقوف ثم تسقط وتتلاشى بعد مغادرتها، وأعداء حمر يقومون بدوريات ويمكن القضاء عليهم بالقفز من الأعلى.

---

## Français

**Happy Collector** est un jeu de plateforme 3D de 20 niveaux réalisé avec Three.js et jouable dans le navigateur. Il a été développé comme un module d'une activation interactive et ludo-éducative multi-jeux pour enfants aux Émirats arabes unis.

Vous contrôlez un cube jaune souriant sur des parcours de plateformes flottantes. Les blocs jaunes portent des émotions et qualités positives ; les ennemis rouges mobiles portent des émotions et comportements négatifs. Collectez les blocs jaunes, évitez ou écrasez les ennemis rouges, franchissez les obstacles et atteignez la porte du niveau pour avancer.

- Bloc jaune collecté : **+10 points**
- Ennemi rouge écrasé par le dessus pendant la descente : **+5 points**
- Toucher un ennemi rouge ou tomber du parcours coûte une vie
- Une partie commence avec **3 vies**
- Après la perte d'une vie, le niveau actuel recommence en conservant les vies restantes
- Il n'est **pas nécessaire** de collecter tous les blocs jaunes pour terminer un niveau
- Atteindre la porte fait passer au niveau suivant
- Terminer le niveau 20 affiche **MASTER COLLECTOR!**

Les libellés jaunes du jeu sont **BRAVERY, JOY, LOVE, HOPE, PEACE, KINDNESS, CALM, PRIDE, TRUST, HAPPINESS**. Les ennemis rouges utilisent **ANGER, GREED, JEALOUSY, RUDENESS, ENVY, HATE, DESPAIR**.

**Ordinateur :** `A / D` ou flèches gauche/droite pour se déplacer ; `W`, `Espace` ou flèche haut pour sauter ; molette pour zoomer après le début du déplacement.  
**Mobile :** commandes gauche/droite et saut à l'écran ; pincement à deux doigts pour zoomer après le début du déplacement.

Le jeu comprend des plateformes horizontales et verticales mobiles, des plateformes pendulaires, des séquences de ponts courbes et suspendus, des portes commandées par boutons, des marches relevées par boutons, des plateformes en verre qui se fissurent lorsqu'on se tient dessus, restent solides tant qu'elles sont occupées, puis tombent et disparaissent après leur départ, ainsi que des ennemis rouges en patrouille pouvant être écrasés.

---

## 简体中文

**Happy Collector** 是一款使用 Three.js 制作、可直接在浏览器中游玩的 20 关 3D 平台游戏。它作为阿联酋儿童多游戏互动寓教于乐活动中的一个游戏模块开发。

玩家控制一个微笑的黄色方块，在漂浮的平台路线中前进。黄色方块代表积极情绪与品质；移动的红色敌人代表消极情绪与行为。收集黄色方块获得分数，避开或从上方踩掉红色敌人，通过平台机关并到达关卡终点的门，即可进入下一关。

- 收集黄色方块：**+10 分**
- 下落时从上方踩掉红色敌人：**+5 分**
- 碰到红色敌人或跌出路线会失去一条生命
- 每局开始时有 **3 条生命**
- 失去一条生命后会重新开始当前关卡，并保留剩余生命
- 完成关卡**不要求**收集全部黄色方块
- 到达关卡终点的门即可进入下一关
- 完成第 20 关后显示 **MASTER COLLECTOR!**

黄色方块使用的英文词语是 **BRAVERY, JOY, LOVE, HOPE, PEACE, KINDNESS, CALM, PRIDE, TRUST, HAPPINESS**。红色敌人使用 **ANGER, GREED, JEALOUSY, RUDENESS, ENVY, HATE, DESPAIR**。

**电脑：** `A / D` 或左右方向键移动；`W`、空格键或上方向键跳跃；开始移动后可使用鼠标滚轮缩放。  
**手机：** 使用屏幕上的左右移动与跳跃按钮；开始移动后可双指缩放。

游戏包含水平和垂直移动平台、摆动平台、弧形桥与绳桥平台序列、按钮控制的闸门、按钮升起的台阶、站上去会裂开但在玩家停留期间保持实体并在离开后坠落淡出的玻璃平台，以及可从上方踩掉的巡逻红色敌人。

---

## Implementation

- `index.html` — complete playable game and runtime logic
- `libs/three.r128.min.js` — local Three.js r128 runtime
- `libs/THREE_LICENSE.txt` — bundled Three.js license
- `music/` — six local music tracks
- `sfx/` — local cinematic wind audio
- `fonts/` — local fonts
- `docs/` — level-expansion rules and pre-delivery QA documentation

The playable runtime loads Three.js locally rather than from a CDN. Most gameplay SFX are synthesized at runtime with the Web Audio API; the cinematic wind is a local audio file.

## Event activation

Happy Collector was developed as one module in a multi-game interactive children's edutainment activation in the UAE.

Event production: [Peach Society](https://peach-society.com/) — Dubai-based event and experiential production company.

## Licensing

The repository currently does **not** declare a project-wide license. The bundled Three.js license applies to Three.js; it should not be interpreted as automatically licensing the Happy Collector game code, artwork, audio, fonts, or other project assets.
