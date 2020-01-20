## Déplace-toi dans ton monde

Le sprite `joueur` doit être capable de marcher à travers les portes dans d'autres salles.

Ton projet contient des arrières-plans pour des salles supplémentaires :

![capture d'écran](images/world-backdrops.png)

\--- task \---

Crée une nouvelle variable 'pour toute les sprites' appelées `salle`{:class="block3variables"} pour savoir dans quelle pièce se trouve le sprite `joueur`.

[[[generic-scratch3-add-variable]]]

![screenshot](images/world-room.png)

\--- /task \---

\--- task \---

When the `player` sprite touches the orange door in the first room, the game should display the next backdrop, and the `player` sprite should move back to the left side of the Stage. Add this code inside the `player` sprite's `forever`{:class="block3control"} loop:

![player](images/player.png)

```blocks3
lorsque le drapeau est cliqué
répéter indéfiniment
    si <touche (flèche haut v) pressée ? > alors
        s'orienter en direction de (0)
        avancer de (4) pas
    end
    si <touche (flèche gauche v) pressée ? > alors
        s'orienter en direction de (-90)
        avancer de (4) pas
    end
        si <touche (flèche bas v) pressée ? > alors
        s'orienter dans la direction (-180)
        avancer de (4) pas
    end
        si <touche [flèche droite v] pressée ? > alors
s'orienter dans la direction (90)
avancer de (4) pas
fin
si < couleur [#BABABA] touchée ? > alors
    avancer de (-4) pas
    end
+ si < couleur [#F2A24A] touchée ? > alors
    basculer sur l'arrière plan (arrière-plan suivant v)
    aller à x: (-200) y: (0)
    ajouter (1) à [salle v]
    end
end
```

\--- /task \---

\--- task \---

Every time the game starts, the room, character position, and backdrop need to be reset.

Add code to the **start** of your `player` sprite code above the `forever`{:class="block3control"} loop, to reset everything when the flag is clicked:

\--- hints \---

\--- hint \---

When the game starts:

+ La valeur de `salle`{:class="block3variables"} doit être définie sur `1`{:class="block3variables"}
+ `L'arrière-plan`{:class="block3looks"} doit être définie sur `salle1`{:class="block3looks"}
+ The position of the `player` sprite should be set to `x: -200 y: 0`{:class="block3motion"}

\--- /hint \---

\--- hint \---

Here are the extra blocks you need:

![player](images/player.png)

```blocks3
aller à x: (-200) y: (0)

ajouter (1) à [salle v]

basculer sur l'arrière-plan (salle1 v)
```

\--- /hint \---

\--- hint \---

Here's what your finished script should look like:

![player](images/player.png)

```blocks3
lorsque le drapeau est cliqué
+ ajouter (1) à [salle v]
+ aller à x: (-200) y: (0)
+ basculer sur l'arrière-plan (salle1 v)
répéter indéfiniment
    si <touche (flèche haut v) pressée ? > alors
        s'orienter en direction de (0)
        avancer de (4) pas
    end
    si <touche (flèche gauche v) pressée? > alors
        s'orienter en direction de (-90)
        avancer de (4) pas
    end
        si <touche (flèche bas v) pressée? > alors
        s'orienter en direction de (-180)
        avancer de (4) pas
    end
        si <touche [flèche droite v] pressée ? > alors
        s'orienter en direction de (90)
        avancer de (4) pas
    end
    si < couleur [#BABABA] touchée ? > alors
    avancer de (-4) pas
    end
    si < couleur [#F2A24A] touchée ? > alors
    basculer sur l'arrière-plan (arrière-plan suivant v)
    aller à x: (-200) y: (0)
    ajouter (1) à [salle v]
end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Click the flag, and then move your `player` sprite until it touches the orange door. Does the sprite move to the next screen? Does the `room`{:class="block3variables"} variable change to `2`?

![screenshot](images/world-room-test.png)

\--- /task \---