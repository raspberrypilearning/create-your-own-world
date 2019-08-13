## Muri solidi

\--- attività \--- Prova di nuovo il tuo sprite `player`. Vedi che può camminare attraverso le pareti grigio chiaro.

![schermata](images/world-walls.png) \--- /task \---

\--- task \--- Per risolvere questo problema, devi far sì che lo sprite `giocatore` si sposti indietro se tocca una parete grigia leggera. Ecco il codice che devi aggiungere all'interno del tuo blocco `forever`{:class="block3control"} sotto i blocchi di direzione:

![player](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
    if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
        if <key (down arrow v) pressed? > then
        point in direction (-180)
        move (4) steps
    end
        if <key [right arrow v] pressed? > then
        point in direction (90)
        move (4) steps
    end
+   if < touching color [#BABABA]? > then
    move (-4) steps
    end
end
```

\--- /task \---

\--- task \---

Prova a far scorrere lo sprite `player` attraverso una parete. Se il nuovo codice funziona, non dovrebbe essere possibile.

![screenshot](images/world-walls-test.png) \--- /task \---