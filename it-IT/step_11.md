## Porte e chiavi

Cosa succede se alcune porte del tuo mondo sono chiuse e il giocatore deve trovare la chiave per aprirle?

+ Seleziona lo sprite `chiave`. Fai click con il tasto destro del mouse su di esso e seleziona **mostra** in modo che appaia sullo schermo.

+ Modifica il costume dello sprite `chiave` in modo che sia blu.

+ Passa alla stanza 3 cambiando sfondo dallo stage e posiziona lo sprite `chiave` in qualche punto difficile da raggiungere!
    
    ![screenshot](images/world-key.png)

+ Aggiungi del codice allo sprite `chiave` in modo che sia visibile solo nella stanza 3.

+ Crea una nuova variabile lista chiamata `inventario`{:class="blockdata"}. Qui è dove verranno memorizzati tutti gli oggetti che il tuo sprite `giocatore` raccoglie.

[[[generic-scratch-make-list]]]

+ Il codice per raccogliere la chiave è molto simile al codice per raccogliere le monete. La differenza è che aggiungi la chiave al tuo inventario.

```blocks
    quando si clicca su ⚑
	attendi fino a quando <sta toccando [giocatore v]>
	aggiungi [chiave blu] a [inventario v]
	ferma [tutti gli altri script dello sprite v]
	nascondi
```

+ Prova il tuo sprite `chiave` per vedere se è possibile raccoglierlo e aggiungerlo al tuo inventario. Ricorda di aggiungere del codice al tuo Stage per svuotare il tuo inventario all'inizio del gioco.

```blocks
    cancella (tutto v) da [inventario v]
```

+ Ora aggiungiamo una porta chiusa. Fai click con il pulsante destro del mouse sullo sprite `porta blu` e seleziona **mostra**, quindi posiziona lo sprite nello spazio tra le due pareti.

![screenshot](images/world-door.png)

+ Aggiungi del codice allo sprite `porta blu` per far sì che sia visibile solo nella stanza 3.

+ Lo sprite `porta blu` dovrebbe nascondersi per permettere al tuo sprite `giocatore` di passare una volta raccolta la chiave blu e questa sia presente nell'inventario.

```blocks
    quando si clicca su ⚑
	attendi fino a quando <[inventario v] contiene [chiave blu]>>
	ferma [tutti gli altri script dello sprite v]
	nascondi
```

+ Prova il tuo progetto e controlla se riesci a raccogliere la chiave blu per aprire la porta!