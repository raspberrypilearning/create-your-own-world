## Murs solides

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls.

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Here's the code you need to add inside your `forever`{:class="block3control"} block below the direction blocks:

![player](images/player.png)

```blocks3
lorsque le drapeau est cliqué
répéter indéfiniment 
    si <touche (flèche haut v) pressée ? > alors
        s'orienter en direction de (0)
        avancer de (4) pas
    end
si <touche (flèche de gauche v) pressée ? > alors
        s'orienter en direction de (-90)
        avancer de (4) pas
    end
        si < touche (flèche du bas v) pressée ? > alors
        s'orienter en direction de (-180)
        avancer de (4) pas
    end
        si <touche [flèche de droite v] pressée? > alors
        s'orienter en direction de (90)
        avancer de (4) pas
    end
+ si < couleur [#BABABA] touchée ? > alors
    avancer de (-4) pas
    end
end
```

\--- /task \---

\--- task \---

Try to make the `player` sprite move through a wall. If your new code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)

\--- /task \---