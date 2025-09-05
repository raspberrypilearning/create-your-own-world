## Défi : ajoute un ennemi

Si tu le souhaites, tu peux également ajouter des ennemis en patrouille à ton jeu. Si le sprite `joueur` touche un ennemi, le jeu se termine.

+ Ton jeu contient déjà un sprite `ennemi`. Ajoute du code au sprite `ennemi` pour qu'il n'apparaisse que dans la salle 2.

+ Ajoute du code pour déplacer le sprite `ennemi` et pour terminer le jeu si le sprite `ennemi` touche le sprite `joueur`. C'est plus facile de faire cela dans des blocs de code séparés. Voici à quoi ton code du sprite `ennemi` pourrait ressembler :

```blocks3
when flag clicked
forever
if <(room :: variables)=[2]> then
show
else
hide

when flag clicked
forever
if <touching (player v)?> then
stop [all v]

when flag clicked
go to x: (170) y:(0)
forever
repeat (130)
change x by (-1)
end
repeat (130)
change x by (1)
```

+ Teste ton nouveau code pour t'assurer que: 
    + Le sprite `ennemi` visible uniquement dans la salle 2
    + Le sprite `ennemi` patrouille la salle
    + Le jeu se termine si le sprite `joueur` touche le sprite `ennemi`

Peux-tu créer un autre sprite `ennemi` dans la salle 3 qui patrouille de haut en bas à travers la fente dans le mur ?

![capture d'écran](images/world-enemy2.png)