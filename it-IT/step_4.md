## Segnali

Lo sprite `player` dovrebbe essere in grado di camminare attraverso le porte in altre stanze.

Il tuo progetto contiene sfondi per ulteriori stanze:

![screenshot](images/world-backdrops.png)

\--- task \---

Crea una nuova variabile valida 'per tutti gli sprite' chiamata `stanza`{: class="blockdata"}, per definire in quale stanza si trova lo sprite `player`.

[[[generic-scratch3-add-variable]]]

![schermata](images/world-room.png) \--- /task \---

\--- task \--- Quando lo sprite `player` tocca la porta arancione nella prima stanza, bisogna rendere visibile lo sfondo successivo, e lo sprite `player` dove tornare sul lato sinistro della scena. Aggiungi questo codice all'interno del ciclo `forever`{:class="blockcontrol"} dello sprite `player`:

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
    if < touching color [#BABABA]? > then
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

\--- task \--- Ogni volta che inizia il gioco, la stanza, la posizione del personaggio e lo sfondo devono essere ripristinati.

Aggiungi questo codice **all'inizio** del codice del tuo sprite `player` prima del ciclo `forever`{:class="blockcontrol"}, per assicurarti che tutto venga ripristinato quando viene cliccata la bandierina verde:

\--- hints \--- \--- hint \--- All'inizio del gioco:

+ Il valore di `stanza`{:class="block3variabili"} dovrebbe essere impostato a `1`{:class="block3variabili"}
+ Lo `sfondo` {: class = "block3looks"} dovrebbe essere impostato su ` room1 ` {: class = "block3looks"}
+ La posizione del ` giocatore ` dovrebbe essere impostato su ` x: -200 y: 0 ` {: class = "block3motion"} \--- /hint \--- \--- hint \--- Ecco i blocchi extra di cui hai bisogno:

![player](images/player.png)

```blocks3
go to x: (-200) y: (0)

set [room v] to (1)

switch backdrop to (room1 v)
```

\--- /hint \--- \--- hint \--- Ecco come dovrebbe apparire il tuo codice:

![player](images/player.png)

```blocks3
when flag clicked
+set [room v] to (1)
+go to x: (-200) y: (0)
+switch backdrop to (room1 v)
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
    if < touching color [#BABABA]? > then
    move (-4) steps
    end
    if < touching color [#F2A24A] > then
    switch backdrop to (next backdrop v)
    go to x: (-200) y: (0)
    change [room v] by (1)
end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \--- Fai clic sulla bandiera, quindi sposta il tuo sprite `player` fino a toccare la porta arancione. Il tuo sprite passa alla schermata successiva? La variabile `stanza`{:class="blockdata"} cambia il proprio valore a `2`?

![schermata](images/world-room-test.png) \--- /task \---