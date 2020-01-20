## Recullida de monedes

La teva icona de ` jugador ` hauria de ser capaç de recollir monedes a mesura que es mou pel món.

\--- task \--- Afegeix una nova variable anomenada ` monedes ` {: class = "block3variables"} pel teu projecte. \--- /task \---

\--- task \--- Selecciona la icona `moneda ` i fes clic a ** mostra **.

![captura de pantalla](images/coin.png) \--- /task \---

\--- task \--- Afegeix codi a la teva icona de `moneda ` de manera que només aparegui a la sala 1. ![captura de pantalla](images/coin.png)

```blocks3
quan has fet clic a la bandera
per sempre
si <(habitació :: variables) =[1]> llavors
mostra
si no
amaga
```

\--- /task \---

\--- task \---

Afegeix codi a la teva icona ` moneda ` de manera que la icona ` s’amaga ` {: class = "block3looks"} i ` 1 ` {: class = "block3variables"} s'afegeix a les ` monedes ` {: class = "block3variables"} variable un cop la icona del `jugador ` toca la icona `moneda ` per "recollir-lo".

![moneda](images/coin.png)

```blocks3
quan has fet clic a la bandera
espera fins que <touching (player v)?>
canvi [monedes v] per (1)
amaga
atura [altres scripts a la icona v]
```

El codi ` deté altres scripts a la icona ` {: class = "block3control"} és necessari perquè la icona `moneda ` deixi de mostrar-se a la sala 1 un cop ha estat recollida.

\--- /task \---

\--- task \--- Afegeix ara codi a l'escenari per configurar les teves ` monedes ` {: class = "block3variables"} variable a ` 0 ` {: class = "block3variables"} al començament del joc.

![escenari](images/stage.png)

```blocks3
quan fas clic a la bandera
posa [monedes v] a [0]
```

\--- /task \---

\--- task \--- Prova el teu joc. La recollida d'una moneda hauria de canviar la teva puntuació de ` monedes ` a ` 1 ` {: class = "block3variables"}. \--- /task \---