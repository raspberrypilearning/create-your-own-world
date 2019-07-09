## Défi : ajoute un ennemi

Si vous le souhaitez, vous pouvez également ajouter des ennemis en patrouille à votre partie. Si le sprite `joueur` touche un ennemi, la partie se termine.

+ Votre jeu contient déjà un sprite `ennemi`. Ajoute du code au sprite `ennemi` pour qu'il n'apparaisse que dans la salle 2.

+ Ajoutez du code pour déplacer le sprite `ennemi` et pour terminer le jeu si le sprite `ennemi` touche le sprite `joueur`. C'est plus facile de faire cela dans des blocs de code séparés. Voici à quoi ton code du sprite `ennemi` pourrait ressembler :

```blocks3
lorsque l' indicateur cliqué
pour toujours
si <(chambre :: variables) =[2]> puis
montrent
autre
hide

lorsque l' indicateur cliqué
pour toujours
si <touching (player v)?> puis
arrêt [all v]

lorsque l' indicateur cliqués
aller à x: ( 170) y: (0)
pour toujours
répéter (130)
changer x par (-1)
fin
répéter (130)
changer x par (1)
```

+ Testez votre nouveau code pour vous assurer que: 
    + Le `ennemi` sprite visible uniquement dans la salle 2
    + Le `ennemi` sprite patrouille la salle
    + Le jeu se termine si le sprite `joueur` touche le sprite `ennemi`

Peux-tu créer un autre sprite `ennemi` dans la salle 3 qui patrouille de haut en bas à travers la fente dans le mur ?

![capture d’écran](images/world-enemy2.png)