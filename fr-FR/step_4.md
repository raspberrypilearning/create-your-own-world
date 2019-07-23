## Déplace-toi dans ton monde

Le sprite `joueur` doit être capable de marcher à travers les portes dans d'autres salles.

Ton projet contient des arrières-plans pour des salles supplémentaires :

![capture d'écran](images/world-backdrops.png)

\--- task \---

Crée une nouvelle variable 'pour toute les sprites' appelées `salle`{:class="block3variables"} pour savoir dans quelle pièce se trouve le sprite `joueur`.

[[[generic-scratch3-add-variable]]]

![capture d'écran](images/world-room.png) \--- /task \---

\--- task \--- Lorsque le sprite `joueur` touche la porte orange dans la première salle, le jeu devrait afficher l'arrière-plan suivant et le sprite `joueur` devrait revenir à gauche de la scène. Ajoute ce code à l'intérieur du sprite `joueur` la boucle `répéter indéfiniment` {class="block3control"}:

![joueur](images/player.png)

```blocks3
lorsque le drapeau est cliqué
répéter indéfiniment
si <touche (flèche de haut v) pressée ? > alors
s'orienter dans la direction (0)
avancer de (4) pas
fin
si <touche (flèche de gauche v) pressée ? > alors
s'orienter dans la direction (-90)
avancer de (4) pas
fin
si <touche (flèche vers le bas v) pressée ? > alors
s'orienter dans la direction (-180)
avancer de (4) pas
fin
si <touche [flèche de droite v] pressée ? > alors
s'orienter dans la direction (90)
avancer de (4) pas
fin
si < couleur [#BABABA] touchée ? > alors
avancer de (-4) pas
fin
+ si < couleur [#F2A24A] touchée ? > alors
basculer sur l'arrière plan (arrière-plan suivant v)
aller à x: (-200) y: (0)
ajouter (1) à [salle v]
fin
fin
```

\--- /task \---

\--- task \--- Chaque fois que le jeu commence, la pièce, la position du personnage et l'arrière-plan doivent être réinitialisés.

Ajoute du code au **début** de ton code sprite `joueur` au-dessus de la boucle `répéter indéfiniment`{:class="block3control"}, pour tout réinitialiser lorsque le drapeau est cliqué:

\--- hints \--- \--- hint \--- Quand le jeu commence :

+ La valeur de `salle`{:class="block3variables"} doit être définie sur `1`{:class="block3variables"}
+ `L'arrière-plan`{:class="block3looks"} doit être définie sur `salle1`{:class="block3looks"}
+ La position du sprite `joueur` doit être réglé sur `x: -200 y: 0`{: class = "block3motion"} \--- /hint \--- \--- hint \--- Voici les blocs supplémentaires dont tu as besoin:

![joueur](images/player.png)

```blocks3
aller à x: (-200) y: (0)

ajouter (1) à [salle v]

basculer sur l'arrière-plan (salle1 v)
```

\--- /hint \--- \--- hint \--- Voici à quoi devrait ressembler ton script terminé:

![joueur](images/player.png)

```blocks3
lorsque le drapeau est cliqué
+ ajouter (1) à [salle v]
+ aller à x: (-200) y: (0)
+ basculer sur l'arrière-plan (salle1 v)
répéter indéfiniment
    si <touche (flèche du haut v) pressée ? > alors
s'orienter dans la direction (0)
avancer de (4) pas
fin
si <touche (flèche de gauche v) pressée? > alors
s'orienter dans la direction (-90)
avancer de (4) pas
fin
si <touche (flèche vers le bas v) pressée? > alors
s'orienter en la direction de (-180)
avancer de (4) pas
fin
si <la touche [flèche de droite v] pressée ? > alors
s'orienter en direction de (90)
avancer de (4) pas
fin
si < couleur [#BABABA] touchée ? > alors
avancer de (-4) pas
fin
si < couleur [#F2A24A] touchée ? > alors
basculer sur l'arrière-plan (arrière-plan suivant v)
aller à x: (-200) y: (0)
ajouter (1) à [salle v]
fin
fin
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \--- Clique sur le drapeau, puis déplace ton sprite `joueur` jusqu'à ce qu'il touche la porte orange. Le sprite passe-t-il à l'écran suivant? La variable `salle`{:class="block3variables"} passe-t-elle à `2`?

![capture d'écran](images/world-room-test.png) \--- /task \---