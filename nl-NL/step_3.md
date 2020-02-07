## Stevige muren

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls.

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Here's the code you need to add inside your `forever`{:class="block3control"} block below the direction blocks:

![player](images/player.png)

```blocks3
wanneer groene vlag wordt aangeklikt
herhaal 
  als <toets (pijltje omhoog v) ingedrukt? > dan
            richt naar (0) graden
            neem (4) stappen
        einde
        als <toets (pijltje links v) ingedrukt? > dan
            richt naar (-90) graden
            neem (4) stappen
        einde
        als <toets (pijltje omlaag v) ingedrukt? > then
        point in direction (-180)
        move (4) steps
    end
        if <key (right arrow v) pressed? > dan
            richt naar (90) graden
            neem (4) stappen
        einde
+ als < raak ik kleur [#BABABA]? > dan 
  neem (-4) stappen
  einde
einde
```

\--- /task \---

\--- task \---

Try to make the `player` sprite move through a wall. If your new code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)

\--- /task \---