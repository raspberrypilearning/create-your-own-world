## Défi: ajoute un ennemi

Si tu le souhaites, tu peux également ajouter des ennemis en patrouille à ton jeu. Si le sprite `joueur` touche un ennemi, le jeu se termine.

+ Ton jeu contient déjà un sprite `ennemi`. Ajoute du code au sprite `ennemi` pour qu'il n'apparaisse que dans la salle 2.

+ Ajoute du code pour déplacer le sprite `ennemi` et pour terminer le jeu si le sprite `ennemi` touche le sprite `joueur`. C'est plus facile de faire cela dans des blocs de code séparés. Voici à quoi ton code du sprite `ennemi` pourrait ressembler:

```blocks3
lorsque le drapeau est cliqué
répéter indéfiniment
si <(salle :: variables) =[2]> alors
montrer
sinon
cacher

lorsque le drapeau est cliqué
répéter indéfiniment
si < touche le (joueur v) ?> alors
stop [tout v]

lorsque le drapeau est cliqué
aller à x: ( 170) y: (0)
répéter indéfiniment
répéter (130)
ajouter (-1) à x
fin
répéter (130) fois
ajouter (1) à x
```

+ Teste ton nouveau code pour t'assurer que: 
    + Le sprite `ennemi` visible uniquement dans la salle 2
    + Le sprite `ennemi` patrouille la salle
    + Le jeu se termine si le sprite `joueur` touche le sprite `ennemi`

Peux-tu créer un autre sprite `ennemi` dans la salle 3 qui patrouille de haut en bas à travers la fente dans le mur?

![capture d’écran](images/world-enemy2.png)