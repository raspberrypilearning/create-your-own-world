## Solidne ściany

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls.

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Here's the code you need to add inside your `forever`{:class="block3control"} block below the direction blocks:

![player](images/player.png)

```blocks3
kiedy kliknięto zieloną flagę
zawsze
    jeżeli <klawisz (strzałka w górę v) naciśnięty? > to
        ustaw kierunek na (0)
        przesuń o (4) kroki
    koniec
    jeżeli <klawisz (strzałka w lewo v) naciśnięty? > to
        ustaw kierunek na (-90)
        przesuń o (4) kroki
    koniec
        jeżeli <klawisz (strzałka w dół v) naciśnięty? > then
        point in direction (-180)
        move (4) steps
    end
        if <key (right arrow v) pressed? > to
        ustaw kierunek na (90)
        przesuń o (4) kroki
    koniec
+   jeżeli < dotyka koloru [#BABABA]? > to
    przesuń o (-4) kroków
    koniec
koniec
```

\--- /task \---

\--- task \---

Try to make the `player` sprite move through a wall. If your new code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)

\--- /task \---