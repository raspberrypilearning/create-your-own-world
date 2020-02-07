## Massive Wände

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls.

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Here's the code you need to add inside your `forever`{:class="block3control"} block below the direction blocks:

![player](images/player.png)

```blocks3
Wenn die grüne Flagge angeklickt
wiederhole fortlaufend 
  falls <Taste (Pfeil nach oben v) gedrückt?> , dann      setze Richtung auf (0) Grad
    gehe (4) er Schritt
  end
  falls <Taste (Pfeil nach links v) gedrückt?> , dann     setze Richtung auf (-90) Grad
    gehe (4) er Schritt
  end
  falls <Taste (Pfeil nach unten v) gedrückt?> , dann  > then
        point in direction (-180)
        move (4) steps
    end
        if <key (right arrow v) pressed?     setze Richtung auf (90) Grad
    gehe (4) er Schritt
  end
  + falls <wird Farbe [#BABABA] berührt?> , dann    +   gehe (-4) er Schritt
  + end
end
```

\--- /task \---

\--- task \---

Try to make the `player` sprite move through a wall. If your new code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)

\--- /task \---