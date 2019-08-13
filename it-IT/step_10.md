## Raccogliere monete

Il tuo sprite `giocatore` dovrebbe essere in grado di raccogliere monete quando si muove nel mondo.

\--- task \--- Aggiungi una nuova variabile denominata ` monete ` {: class = "block3variables"} al tuo progetto. \--- /task \---

\--- task \--- Seleziona lo sprite `monete` e clicca **mostra**.

![schermata](images/coin.png) \--- /task \---

\--- task \--- Aggiungi del codice allo sprite `moneta` per far sì che appaia solo nella stanza 1. ![schermata](images/coin.png)

```blocks3
when flag clicked
forever
if <(room :: variables)=[1]> then
show
else
hide
```

\--- /task \---

\--- task \---

Aggiungi del codice allo sprite `moneta` per far sì che `1` venga aggiunto alle variabile `monete`{:class="blockdata"} una volta che lo sprite `giocatore ` tocca lo sprite `moneta` per "raccoglierla".

![moneta](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

Il codice `ferma tutti gli altri script dello sprite`{:class="blockcontrol"} è necessario affinchè lo sprite `moneta` smetta di essere visualizzato nella stanza 1 una volta che è stato raccolto.

\--- /task \---

\--- task \--- Ora aggiungi il codice per impostare le tue `monete`{:class="block3variabili"} a `0`{:class="block3variabili"} all'inizio del gioco.

![schermo](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

\--- /task \---

\--- task \--- Prova il tuo gioco. La raccolta di una moneta deve cambiare le ` monete ` a ` 1 ` {: Class = "block3variables"}. \--- /task \---