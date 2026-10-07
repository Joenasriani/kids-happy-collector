# Happy Collector: 20-Level Three.js Browser Platformer

<p align="center">
  <img src="assets/readme/happy-collector-banner.png" alt="Happy Collector" width="100%">
</p>

<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.ar.md">العربية</a> ·
  <a href="README.fr.md">Français</a> ·
  <a href="README.zh-CN.md">简体中文</a>
</p>

**Play:** https://kids-happy-collector.vercel.app/  
**Itch.io:** https://joenasr.itch.io/happy-collector

## Français

**Happy Collector** est un jeu de plateforme 3D de 20 niveaux réalisé avec Three.js et jouable dans le navigateur. Il a été développé comme un module d'une activation interactive et ludo-éducative multi-jeux pour enfants aux Émirats arabes unis.

Vous contrôlez un cube jaune souriant sur des parcours de plateformes flottantes. Les blocs jaunes portent des émotions et qualités positives ; les ennemis rouges mobiles portent des émotions et comportements négatifs. Collectez les blocs jaunes, évitez ou écrasez les ennemis rouges, franchissez les obstacles et atteignez la porte du niveau pour avancer.

## Comment jouer

- Bloc jaune collecté : **+10 points**
- Ennemi rouge écrasé par le dessus pendant la descente : **+5 points**
- Toucher un ennemi rouge ou tomber du parcours coûte une vie
- Une partie commence avec **3 vies**
- Après la perte d'une vie, le niveau actuel recommence en conservant les vies restantes
- Il n'est **pas nécessaire** de collecter tous les blocs jaunes
- Atteindre la porte fait passer au niveau suivant
- Terminer le niveau 20 affiche **MASTER COLLECTOR!**

Les blocs jaunes utilisent **BRAVERY, JOY, LOVE, HOPE, PEACE, KINDNESS, CALM, PRIDE, TRUST, HAPPINESS**. Les ennemis rouges utilisent **ANGER, GREED, JEALOUSY, RUDENESS, ENVY, HATE, DESPAIR**.

## Commandes

**Ordinateur :** `A / D` ou flèches gauche/droite pour se déplacer ; `W`, `Espace` ou flèche haut pour sauter ; molette pour zoomer après le début du déplacement.  
**Mobile :** commandes gauche/droite et saut à l'écran ; pincement à deux doigts pour zoomer après le début du déplacement.

## Systèmes de jeu

Le jeu comprend des plateformes horizontales et verticales mobiles, des plateformes pendulaires, des séquences de ponts courbes et suspendus, des portes commandées par boutons, des marches relevées par boutons, des plateformes en verre et des ennemis rouges en patrouille. Le verre se fissure lorsque le joueur se tient dessus, reste solide tant qu'il est occupé, puis tombe et disparaît après son départ. Le jeu comprend également plusieurs ambiances de ciel, de la musique, des effets sonores et visuels et des vibrations sur les appareils compatibles.

## Architecture des niveaux

Les 20 niveaux sont construits à partir de définitions réutilisables de plateformes et d'obstacles. Les niveaux 11 à 20 utilisent des séquences définies directement dans le code.

## Implémentation

Le jeu complet et sa logique se trouvent dans `index.html`, avec Three.js r128 chargé localement, ainsi que des ressources musicales, audio, typographiques et de la documentation de niveau/QA. Three.js n'est pas chargé depuis un CDN.

## Contexte du projet

Happy Collector a été développé comme un module d'une activation interactive et ludo-éducative multi-jeux pour enfants aux Émirats arabes unis.

Production de l'événement : [Peach Society](https://peach-society.com/).

## Licence

Le dépôt ne déclare actuellement aucune licence couvrant l'ensemble du projet. La licence Three.js incluse ne s'applique qu'à Three.js et ne doit pas être interprétée comme une licence automatique du code, des graphismes, de l'audio, des polices ou des autres ressources de Happy Collector.
