## Muri solidi

--- task ---

Prova di nuovo il tuo sprite `giocatore`. Do you see that it can walk through the light grey walls?

![schermata](images/world-walls.png)

--- /task ---

--- task ---

Per risolvere questo problema, devi far sì che lo sprite `giocatore` si sposti indietro se tocca una parete grigia leggera. Ecco il codice che devi aggiungere all'interno del tuo blocco `per sempre`{:class="block3control"} sotto i blocchi di direzione:

![giocatore](images/player.png)

```blocks3
when flag clicked
forever
	if <key (freccia su v) pressed? > then
		point in direction (0)
		move (4) steps
	end
	if <key (freccia sinistra v) pressed? > then
		point in direction (-90)
		move (4) steps
	end
		if <key (freccia giu v) pressed? > then
		point in direction (-180)
		move (4) steps
	end
		if <key (right arrow v) pressed? > then
		point in direction (90)
		move (4) steps
	end
+	if < touching color [#BABABA]? > then
	move (-4) steps
	end
end
```

--- /task ---

--- task ---

Prova a far correre lo sprite `giocatore` attraverso una parete. Se il nuovo codice funziona, non dovrebbe essere possibile.

![schermata](images/world-walls-test.png)

--- /task ---