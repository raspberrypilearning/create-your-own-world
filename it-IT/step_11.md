## Porte e chiavi

Ora aggiungerai il codice in modo che alcune porte del tuo mondo di gioco siano bloccate e il giocatore debba trovare la chiave per aprirle e passare alla stanza successiva.

--- task ---

Seleziona lo sprite `chiave`. Fai clic su `mostra`{:class="blocklooks"} nel menu codice in modo che lo sprite appaia sullo stage.

--- /task ---

--- task ---

Modifica il costume dello sprite `chiave` in modo che sia blu.

--- /task ---

--- task ---

Passa alla stanza 3 cambiando sfondo dallo stage e posiziona lo sprite `chiave` in qualche punto difficile da raggiungere!

![schermata](images/world-key.png)

--- /task ---

--- task ---

Aggiungi del codice allo sprite `chiave` in modo che sia visibile solo nella stanza 3.

--- /task ---

--- task ---

Crea una nuova lista chiamata `inventario`{:class="block3variables"} per memorizzare gli oggetti che lo sprite `giocatore` colleziona.

[[[generic-scratch3-make-list]]]

--- /task ---

--- task ---

Il codice che è necessario aggiungere per raccogliere la chiave è molto simile al codice per la raccolta delle monete. La differenza è che aggiungi la chiave all'`inventario`{:class="block3variables"}.

![chiave](images/key.png)

```blocks3
quando si clicca sulla bandiera verde
attendi fino a quando <touching (giocatore v)?>
aggiungi [chiave blu] a [inventario v]
nascondi
ferma [altri script in sprite v]
```

--- /task ---

--- task ---

Aggiungi il codice per svuotare il tuo inventario all'inizio del gioco.

```blocks3
delete all of [inventario v]
```

--- /task ---

--- task ---

Prova il tuo gioco per verificare se è possibile raccogliere lo sprite `chiave` e aggiungerlo al tuo inventario.

--- /task ---

--- task ---

Ora aggiungiamo una porta chiusa. Seleziona lo sprite `porta blu` e clicca su `mostra`{:class="blocklooks"} nel menu codice, e quindi posiziona lo sprite nel passaggio tra le due pareti.

![schermata](images/world-door.png)

--- /task ---

--- task ---

Aggiungi del codice allo sprite `porta blu` per far sì che sia visibile solo nella stanza 3.

--- /task ---

--- task ---

Aggiungi il codice a `porta blu` in modo che, quando la chiave si trova nell'`inventario`{:class="block3variables"}, lo sprite sia `nascosta`{:class="block3looks"} per consentire al tuo `giocatore` di passare.

![porta](images/door.png)

```blocks3
quando si clicca sulla bandiera verde
attendi fino a quando <[inventario v] contiene [chiave blu]?>
ferma [altri script in sprite v]
nascondi
```

--- /task ---

--- task ---

Prova il tuo progetto e controlla se riesci a raccogliere la chiave blu per aprire la porta!

--- /task ---