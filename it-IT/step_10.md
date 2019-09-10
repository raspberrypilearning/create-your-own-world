## Raccogliere monete

Il tuo sprite `player` dovrebbe essere in grado di raccogliere monete quando si muove nel mondo.

\--- task \--- Aggiungi una nuova variabile denominata `monete` {:class="block3variables"} al tuo progetto. \--- /task \---

\--- task \--- Seleziona lo sprite `monete` e clicca **mostra**.

![schermata](images/coin.png) \--- /task \---

\--- task \--- Aggiungi del codice allo sprite `moneta` per far sì che appaia solo nella stanza 1. ![schermata](images/coin.png)

```blocks3
quando si clicca sulla bandiera verde
per sempre 
 se <(stanza :: variables) = [1]> allora 
 mostra
 altrimenti 
 nascondi
 end
end
```

\--- /task \---

\--- task \---

Aggiungi del codice allo sprite `moneta` per fare in modo che `scompaia<code> ed il valore <code>1` venga aggiunto alle variabile `monete`{:class="blockdata"} quando lo sprite `player` tocca lo sprite <0>moneta</code> per "raccoglierla".

![moneta](images/coin.png)

```blocks3
quando si clicca sulla bandiera verde
attendi fino a quando <touching (player v)?>
cambia [monete v] di (1)
nascondi
ferma [altri script in sprite v]
```

Il codice `ferma tutti gli altri script dello sprite`{:class="blockcontrol"} è necessario affinchè lo sprite `moneta` smetta di essere visualizzato nella stanza 1 una volta che è stato raccolto.

\--- /task \---

\--- task \--- Ora aggiungi il codice per impostare le tue `monete`{:class="block3variabili"} a `0`{:class="block3variabili"} all'inizio del gioco.

![stage](images/stage.png)

```blocks3
quando si clicca sulla bandiera verde
porta [monete v] a [0]
```

\--- /task \---

\--- task \--- Prova il tuo gioco. La raccolta di una moneta deve cambiare il valore delle `monete` a `1` {:class="block3variables"}. \--- /task \---