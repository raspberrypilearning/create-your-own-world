## Recollida de monedes

El teu personatge `jugador` hauria de ser capaç de recollir monedes a mesura que es mou pel món.

--- task ---

Afegeix una nova variable anomenada `monedes`{:class="block3variables"} pel teu projecte.

--- /task ---

--- task ---

Selecciona el personatge `moneda` i fes clic a **mostra**.

![captura de pantalla](images/coin.png)

--- /task ---

--- task ---

Afegeix codi al teu personatge `moneda` de manera que només aparegui a l'habitació 1.

![captura de pantalla](images/coin.png)

```blocks3
when flag clicked
per sempre
si <(habitació :: variables) =[1]> llavors
mostra't
si no
amaga't
```

--- /task ---

--- task ---

Afegeix codi al teu personatge `moneda` de manera que el personatge `s’amagui`{:class="block3looks"} i suma `1`{:class="block3variables"} a la variable `monedes`{:class="block3variables"} un cop el personatge del `jugador` toqui el personatge `moneda` per "recollir-la".

![moneda](images/coin.png)

```blocks3
when flag clicked
espera fins <touching (jugador v)?>
change [monedes v] by (1)
amaga't
atura [altres programes del personatge v]
```

El codi `atura altres programes del personatge`{:class="block3control"} és necessari perquè el personatge `moneda` deixi de mostrar-se a l'habitació 1 un cop ha estat recollida.

--- /task ---

--- task ---

Afegeix ara codi a l'Escenari per assignar a la teva variable `monedes`{:class="block3variables"} el valor `0`{:class="block3variables"} al començament del joc.

![escenari](images/stage.png)

```blocks3
when flag clicked
set [monedes v] to [0]
```

--- /task ---

--- task ---

Prova el teu joc. La recollida d'una moneda hauria de canviar la teva puntuació de `monedes` a `1`{:class="block3variables"}.

--- /task ---