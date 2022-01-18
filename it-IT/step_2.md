## Codifica il tuo giocatore

Inizia creando uno sprite `giocatore` che possa muoversi nel mondo.

--- task ---

Apri il progetto di avvio Scratch 'Crea il tuo mondo'.

**Online:** apri il progetto iniziale su [scratch.mit.edu/projects/395751322](https://scratch.mit.edu/projects/395751322){:target="_blank"}.

Se hai un account su Scratch, puoi farne una copia cliccando su **Remix**.

**Offline:** scarica il progetto iniziale da [rpf.io/p/it-IT/create-your-own-world-go](https://rpf.io/p/it-IT/create-your-own-world-go){:target="_blank"}, e aprilo con l'editor offline. Se hai bisogno di scaricare ed installare l'editor Scratch offline, puoi trovarlo su [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![schermata](images/world-starter.png)

--- /task ---

Premendo i tasti freccia si dovrà spostare lo sprite `giocatore` intorno. Quando si preme la freccia su, lo sprite `giocatore` in risposta dovrebbe spostarsi verso l'alto dello stage.

--- task ---

Aggiungi questo codice allo sprite `giocatore`:

![giocatore](images/player.png)

```blocks3
quando si clicca sulla bandiera verde
per sempre 
  se <tasto (freccia su v) premuto? > allora 
    punta in direzione (0)
    fai (4) passi
  end
end
```

--- /task ---

--- task ---

Fai clic sulla bandiera e tieni premuta la freccia su. Il tuo sprite `giocatore` si muove verso l'alto?

![schermata](images/world-up.png)

--- /task ---

--- task ---

Per spostare lo sprite `giocatore` a sinistra, è necessario aggiungere un altro blocco `se`{:class="blockcontrol"} con un codice simile a quello precedente:

![giocatore](images/player.png)

```blocks3
when flag clicked
forever
	if <key (freccia su v) pressed? > then
		point in direction (0)
		move (4) steps
	end
+	if <key (freccia sinistra v) pressed? > then
		point in direction (-90)
		move (4) steps
	end
end
```

--- /task ---

--- task ---

Aggiungi altro codice al tuo sprite `giocatore` in modo che possa muoversi anche verso destra e verso il basso. Usa il codice che hai già per aiutarti.

--- hints ---


--- hint ---

Per spostarti verso l'alto, punta `giocatore` in direzione `0` gradi. Cosa dovresti fare per spostare lo sprite verso il basso?

Per spostarti a sinistra, hai puntato lo sprite in direzione `-90` gradi. Cosa dovresti fare per spostare lo sprite verso destra?

--- /hint ---

--- hint ---

Devi modificare questi due blocchi:

![giocatore](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

Duplica il codice che muove lo sprite `giocatore` verso l'alto e cambia questi due blocchi per far spostare lo sprite verso il basso. Duplica nuovamente il codice e modificalo per spostare lo sprite verso destra.

--- /hint ---

--- hint ---

Il tuo codice dovrebbe essere più o meno così:

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
+    if <key (down arrow v) pressed? > then
		point in direction (180)
		move (4) steps
	end
+    if <key (right arrow v) pressed? > then
		point in direction (90)
		move (4) steps
	end
end
```

--- /hint ---

--- /hints ---

--- /task ---
