## Murs massissos

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls.

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Here's the code you need to add inside your `forever`{:class="block3control"} block below the direction blocks:

![player](images/player.png)

```blocks3
quan has fet clic a la bandera
per sempre
    si has apretat <tecles (fletxa amunt v)? > llavors
        punt de direcció (0)
        moure (4) passes
    final
  si has apretat <tecles (fletxa esquerra v)? > llavors
        punt de direcció (-90)
        moure (4) passes
    final
  si has apretat <tecles (fletxa avall v)? > llavors
        punt de direcció (-180)
        moure (4) passes
    final
  si has apretat <tecles [fletxa dreta v]? > llavors
        punt de direcció (90)
        moure (4) passes
    final
+ si < tocant el color [#BABABA]? > llavors
    moure (-4) passes
    final
final
```

\--- /task \---

\--- task \---

Try to make the `player` sprite move through a wall. If your new code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)

\--- /task \---