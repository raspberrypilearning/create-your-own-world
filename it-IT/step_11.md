## Porte e chiavi

Ora aggiungerai il codice in modo che alcune porte del tuo mondo di gioco siano bloccate e il giocatore deve trovare la chiave per aprirle e passare alla stanza successiva.

\--- task \--- Seleziona lo sprite `chiave`. Fai clic su ` mostra ` {: class = "blocklooks"} nel menu Script in modo che lo sprite appaia sullo stage. \--- /task \---

\--- task \--- Modifica la `chiave` in modo che sia blu. \--- /task \---

\--- task \--- Passa allo sfondo dello stage nella stanza 3 e posiziona `la chiave` in un posto difficile da raggiungere!

![schermata](images/world-key.png)

\--- /task \---

\--- task \--- Aggiungi del codice allo sprite `chiave` in modo che sia visibile solo nella stanza 3. \--- /task \---

\--- task \--- Crea una nuova lista chiamata `inventario`{:class="block3variabili"} per memorizzare gli oggetti che `giocatore` colleziona.

[[[generic-scratch3-make-list]]] \--- /task \---

\--- task \--- Il codice che è necessario aggiungere per raccogliere la chiave è molto simile al codice per la raccolta di monete. La differenza è che aggiungi la chiave all'`inventario` {: Class = "block3variables"}.

![chiave](images/key.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
add [blue key] to [inventario v]
hide
stop [other scripts in sprite v]
```

\--- /task \---

\--- task \--- Aggiungi il codice per svuotare il tuo inventario all'inizio del gioco.

```blocks3
cancella (tutto v) da [inventario v]
```

\--- /task \---

\--- task \--- Prova il tuo gioco per verificare se è possibile raccogliere lo sprite `chiave` e aggiungerlo al tuo inventario. \--- /task \---

\--- task \--- Ora aggiungi la porta bloccata. Seleziona lo sprite `door-blue` e clicca su `mostra`{:class="blocklook} nel menu Scripts, e quindi posiziona lo sprite attraverso il divario tra le due pareti.

![schermata](images/world-door.png) \--- /task \---

\--- task \--- Aggiungi il codice a ` door-blue ` in modo che sia visibile solo nella stanza 3. \--- /task \---

\--- task \--- Aggiungi il codice a ` door-blue ` in modo che, quando la chiave si trova nell'inventario ` ` {: class = "block3variables"}, lo sprite ` si nasconde ` {: class = "block3looks"} per consentire al tuo ` giocatore ` di passare.

![porta](images/door.png)

```blocks3
when flag clicked
wait until <[inventario v] contains [blue key]?>
stop [other scripts in sprite v]
hide
```

\--- /task \---

\--- task \--- Prova il tuo gioco e vedi se riesci a raccogliere la chiave blu per aprire la porta! \--- /task \---