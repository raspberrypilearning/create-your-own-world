## Programmare il tuo mondo

Permettiamo allo sprite `giocatore` di camminare attraverso le porte verso altre stanze.

Il tuo progetto contiene sfondi per ulteriori stanze:

![screenshot](images/world-backdrops.png)

+ Crea una nuova variabile valida 'per tutti gli sprite' chiamata `stanza`{: class="blockdata"}, per definire in quale stanza si trova lo sprite `giocatore`.

[[[generic-scratch-add-variable]]]

![screenshot](images/world-room.png)

+ Quando lo sprite `giocatore` tocca la porta arancione nella prima stanza, bisogna rendere visibile lo sfondo successivo, e lo sprite `giocatore` dove tornare sul lato sinistro della scena. Aggiungi questo codice all'interno del ciclo `per sempre`{:class="blockcontrol"} dello sprite `giocatore`:

```blocks
    se < sta toccando il colore [#F2A24A] > allora 
        passa allo sfondo [sfondo successivo v]
        vai a x: (-200) y: (0)
        cambia [stanza v] di (1)
    fine
```

+ Aggiungi questo codice **all'inizio** del codice del tuo sprite `giocatore` (prima del ciclo `per sempre`{:class="blockcontrol"}), per assicurarti che tutto venga ripristinato quando viene cliccata la bandierina verde:
    
    ```blocks
        porta [stanza v] a (1)
        vai a x: (-200) y: (0)
        passa allo sfondo [stanza 1 v]
    ```

+ Fai click sulla bandierina verde e sposta il tuo sprite `giocatore` sopra la porta arancione. Il tuo sprite passa alla schermata successiva? La variabile `stanza`{:class="blockdata"} cambia il proprio valore a `2`?

![screenshot](images/world-room-test.png)

\--- challenge \---

### Sfida: trasferirsi nella stanza precedente

+ Riesci a fare in modo che il tuo sprite `giocatore` torni nella stanza precedente dopo aver toccato una porta gialla? Il codice necessario per fare ciò è molto simile al codice che hai già aggiunto per far passare il giocatore alla stanza successiva.

\--- /challenge \---