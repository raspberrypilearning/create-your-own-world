## Segnali

Lo sprite `player` dovrebbe essere in grado di raggiungere altre stanze attraversando le porte.

Il tuo progetto contiene sfondi per ulteriori stanze:

![screenshot](images/world-backdrops.png)

\--- task \---

Crea una nuova variabile valida 'per tutti gli sprite' chiamata `stanza`{:class="blockdata"}, per definire in quale stanza si trova lo sprite `player`.

[[[generic-scratch3-add-variable]]]

![screenshot](images/world-room.png)

\--- /task \---

\--- task \---

Quando lo sprite `player` tocca la porta arancione nella prima stanza, bisogna rendere visibile lo sfondo successivo, e lo sprite `player` deve tornare sul lato sinistro dello stage. Aggiungi questo codice all'interno del ciclo `per sempre`{:class="block3control"} dello sprite `player`:

![player](images/player.png)

```blocks3
quando si clicca sulla bandiera verde
per sempre 
  se <tasto (freccia su v) premuto? > allora 
    punta in direzione (0)
    fai (4) passi
  end
  se <tasto (freccia sinistra v) premuto? >allora 
    punta in direzione (-90)
    fai (4) passi
  end
  se <tasto (freccia giu v) premuto? >allora 
    punta in direzione (-180)
    fai (4) passi
  end
  se <tasto [freccia destra v] premuto? > allora 
    punta in direzione (90)
    fai (4) passi
  end
  se < sta toccando il colore [#BABABA]? > then
    move (-4) steps
    end
+   if < touching color [#F2A24A] > then
    switch backdrop to (next backdrop v)
    go to x: (-200) y: (0)
    change [room v] by (1)
    end
end
```

\--- /task \---

\--- task \---

Ogni volta che inizia il gioco, la stanza, la posizione del personaggio e lo sfondo devono essere ripristinati.

Aggiungi questo codice **all'inizio** del codice del tuo sprite `player` prima del ciclo `per sempre`{:class="block3control"}, per assicurarti che tutto venga ripristinato quando viene cliccata la bandierina verde:

\--- hints \---

\--- hint \---

Quando si avvia il gioco:

+ Il valore di `stanza`{:class="block3variabili"} dovrebbe essere impostato a `1`{:class="block3variabili"}
+ Lo `sfondo` {:class="block3looks"} dovrebbe essere impostato su ` stanza1 ` {:class="block3looks"}
+ La posizione del `giocatore` deve essere impostata a `x: -200 y: 0`{:class="block3motion"}

\--- /hint \---

\--- hint \---

Ecco i blocchi di codice che ti serviranno:

![player](images/player.png)

```blocks3
vai a x: (-200) y: (0)

porta [stanza v] a (1)

passa allo sfondo (stanza1 v)
```

\--- /hint \---

\--- hint \---

Ecco come dovrebbe apparire il risultato:

![player](images/player.png)

```blocks3
quando si clicca sulla bandiera verde
+porta [stanza v] a (1)
+vai a x: (-200) y: (0)
+passa allo sfondo (stanza1 v)
per sempre 
se <tasto (freccia su v) premuto? > allora 
    punta in direzione (0)
    fai (4) passi
  end
  se <tasto (freccia sinistra v) premuto? >allora 
    punta in direzione (-90)
    fai (4) passi
  end
  se <tasto (freccia giu v) premuto? >allora 
    punta in direzione (-180)
    fai (4) passi
  end
  se <tasto [freccia destra v] premuto? > allora 
    punta in direzione (90)
    fai (4) passi
  end
  se < sta toccando il colore [#BABABA]? > allora 
    fai (-4) passi
  end
  se < sta toccando il colore [#F2A24A]> allora 
    passa allo sfondo (next backdrop v)
    vai a x: (-200) y: (0)
    cambia [stanza v] di (1)
  end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Fai clic sulla bandiera, quindi sposta il tuo sprite `player` fino a toccare la porta arancione. Il tuo sprite passa alla schermata successiva? La variabile `stanza`{:class="block3variables"} cambia il proprio valore a `2`?

![schermata](images/world-room-test.png)

\--- /task \---