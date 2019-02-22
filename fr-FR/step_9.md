## Challenge: ajoute un ennemi

If you want, you can also add patrolling enemies to your game. If the `player` sprite touches an enemy, the game ends.

+ Your game already contains an `enemy` sprite. Ajouter du code au lutin `ennemi` pour qu'il n'apparaisse que dans la salle 2.

+ Add code to move the `enemy` sprite and to end the game if the `enemy` sprite touches the `player` sprite. C'est plus facile de faire cela dans des blocs de code séparés. Voici à quoi ton code du lutin `ennemi` pourrait ressembler:

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

+ Test out your new code to make sure that: 
    + The `enemy` sprite only visible in room 2
    + The `enemy` sprite patrols the room
    + The game ends if the `player` sprite touches the `enemy` sprite

Peux-tu créer un autre lutin `ennemi` dans la salle 3 qui patrouille de haut en bas à travers la fente du mur ?

![screenshot](images/world-enemy2.png)