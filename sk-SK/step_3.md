## Pevné steny

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls.

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Here's the code you need to add inside your `forever`{:class="block3control"} block below the direction blocks:

![player](images/player.png)

```blocks3
keď sa vlajka preklikne
navždy
    ak <stlačíte tlačidlo (šípka nahor v)? > potom
        bod v smere (0)
        posunúť (4) kroky
    koniec
    ak je stlačené tlačidlo <(šípka doľava v)? > potom
        bod v smere (-90)
        posunúť (4) kroky
    koniec
        ak stlačíte klávesu <(šípka dole v)? > potom
        bod v smere (-180)
        posunúť (4) kroky
    koniec
        ak je stlačené tlačidlo <[šípka vpravo v]? > potom
        bod v smere (90)
        posunúť (4) kroky
    koniec
+ ak < dotýkať farbu [#BABABA]? > potom
    krok (-4) kroky
    koniec
koniec
```

\--- / úloha \---

\--- task \---

Try to make the `player` sprite move through a wall. If your new code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)

\--- /task \---