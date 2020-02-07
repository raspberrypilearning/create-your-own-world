## Muri solidi

\--- task \---

Prova di nuovo il tuo sprite `giocatore`. Vedi che può camminare attraverso le pareti grigio chiaro.

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

Per risolvere questo problema, devi far sì che lo sprite `giocatore` si sposti indietro se tocca una parete grigia leggera. Ecco il codice che devi aggiungere all'interno del tuo blocco `per sempre`{:class="block3control"} sotto i blocchi di direzione:

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
  se <tasto (freccia giu v) premuto? > then
        point in direction (-180)
        move (4) steps
    end
        if <key (right arrow v) pressed? > allora 
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

Prova a far correre lo sprite `player` attraverso una parete. Se il nuovo codice funziona, non dovrebbe essere possibile.

![schermata](images/world-walls-test.png)

\--- /task \---