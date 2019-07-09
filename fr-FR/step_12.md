## Défi : étends ton monde

Tu peux maintenant continuer à créer ton propre monde ! Voici quelques idées :

+ Ajoutez plus de pièces à votre jeu dans différentes pièces. Pouvez-vous laisser des pièces en gardant les ennemis en patrouille?
+ Changer les décors de votre jeu
+ Ajoute du son et de la musique à ton jeu
+ Ajoutez plus de personnes, d'ennemis et de signes
+ Ajoute des portes rouges et jaunes, et des clés spéciales pour les ouvrir
+ Ajoute plus de salles à ton monde
+ Ajoute d'autres objets utiles à ton jeu
    
    + Utilise des pièces pour obtenir des informations d'autres personnes :

![capture d'écran](images/world-bribe.png)

+ Tu pourrais même ajouter des portes dans les murs nord et sud de la salle 1, pour que le joueur puisse se déplacer d'une salle à l'autre dans les quatre directions. Par exemple, votre jeu peut avoir neuf salles dans une grille 3 × 3. Ensuite, tu peux ajouter `3` au numéro de la salle pour descendre d’un niveau.

![capture d'écran](images/north-south-rooms.png) ![capture d'écran](images/number-grid.png)

```blocks3
si <touching color [ ]?> alors
change de décor pour ((costume [numéro v]) + (3))
aller à x: (0) y: (200)
changer [salle v] par (3)
```