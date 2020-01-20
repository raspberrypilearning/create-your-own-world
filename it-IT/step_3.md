## Muri solidi

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls.

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Here's the code you need to add inside your `forever`{:class="block3control"} block below the direction blocks:

![player](images/player.png)

```blocks3
quando si clicca sulla bandiera verde
per sempre 
se <tasto (freccia su v) premuto? > allora 
    punta in direzione (0)
    fai (4) passi
  end
  se <tasto (freccia sinistra v) premuto? > allora 
    punta in direzione (-90)
    fai (4) passi
  end
  se <tasto (freccia giu v) premuto? > allora 
    punta in direzione (-180)
    fai (4) passi
  end
  se <tasto [freccia destra v] premuto? > allora 
    punta in direzione (90)
    fai (4) passi
  end
  + se < sta toccando il colore [#BABABA]? > allora 
  +   fai (-4) passi
  + end
end
```

\--- /task \---

\--- task \---

Try to make the `player` sprite move through a wall. If your new code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)

\--- /task \---