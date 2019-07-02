## Défi : étends ton monde

Tu peux maintenant continuer à créer ton propre monde ! Voici quelques idées :

+ Add more coins to your game in different rooms. Can you let some coins be guarded by patrolling enemies?
+ Change your game's backdrops
+ Ajoute du son et de la musique à ton jeu
+ Add more people, enemies, and signs
+ Ajoute des portes rouges et jaunes, et des clés spéciales pour les ouvrir
+ Ajoute plus de salles à ton monde
+ Ajoute d'autres objets utiles à ton jeu
    
    + Utilise des pièces pour obtenir des informations d'autres personnes :

![capture d'écran](images/world-bribe.png)

+ Tu pourrais même ajouter des portes dans les murs nord et sud de la salle 1, pour que le joueur puisse se déplacer d'une salle à l'autre dans les quatre directions. For example, your game can have nine rooms in a 3×3 grid. Ensuite, tu peux ajouter `3` au numéro de la salle pour descendre d’un niveau.

![capture d'écran](images/north-south-rooms.png) ![capture d'écran](images/number-grid.png)

```blocks3
if <touching color [ ]?> then
switch backdrop to ((costume [number v]) + (3))
go to x:(0) y:(200)
change [room v] by (3)
```