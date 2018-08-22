## Muri solidi

+ Metti di nuovo alla prova lo sprite `giocatore`: probabilmente noterai che ha la capacità di attraversare le pareti color grigio chiaro.

![screenshot](images/world-walls.png)

+ Per risolvere questo problema, devi spostare lo sprite `giocatore` indietro se sta toccando un muro color grigio chiaro. Ecco il codice che dovrai aggiungere all'interno del tuo blocco `per sempre`{:class="blockcontrol"}, sotto il blocco relativo alle direzioni:

```blocks
    se < sta toccando il colore [#BABABA] > allora 
        fai (-4) passi 
    fine
```

+ Prova questo nuovo codice: sposta lo sprite `giocatore` verso il muro, e controlla se è possibile farlo passare attraverso. Se il tuo codice è corretto, non dovrebbe essere possibile farlo.

![screenshot](images/world-walls-test.png)