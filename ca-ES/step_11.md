## Portes i claus

Ara afegiràs codi perquè algunes de les portes del món del joc estiguin bloquejades i el jugador hagi de trobar la clau per obrir-les i arribar a la sala següent.

--- task ---

Canvia al personatge `clau`. Fes clic a `mostra't`{:class="blocklooks"} del menú Codi de manera que el personatge aparegui a l'Escenari.

--- /task ---

--- task ---

Edita el vestit del personatge `clau` perquè quedi de color blau.

--- /task ---

--- task ---

Canvia el fons de l'habitació 3 i posa el personatge de la `clau` en algun lloc difícil d’arribar!

![captura de pantalla](images/world-key.png)

--- /task ---

--- task ---

Afegeix codi al teu personatge de la `clau` de manera que només sigui visible a l'habitació 3.

--- /task ---

--- task ---

Crea una llista nova anomenada `inventari`{:class="block3variables"} per emmagatzemar els articles que el teu personatge `jugador` recull.

[[[generic-scratch3-make-list]]]

--- /task ---

--- task ---

El codi que has d'afegir per recollir la clau és molt similar al codi de recollida de monedes. La diferència és que afegeixes la clau a l'`inventari`{:class="block3variables"}.

![clau](images/key.png)

```blocks3
when flag clicked
espera fins <touching (jugador v)?>
afegeix [clau blava] a [inventari v]
amaga't
atura [altres programes del personatge v]
```

--- /task ---

--- task ---

Afegeix codi al teu Escenari per buidar l’inventari al començament del joc.

```blocks3
esborra-ho tot de [inventari v]
```

--- /task ---

--- task ---

Prova el teu joc per comprovar si pots recollir el personatge de la `clau` i afegir-lo al teu inventari.

--- /task ---

--- task ---

Ara afegeix la porta bloquejada. Selecciona el personatge `porta blava` i fes clic a `mostra't`{:class="blocklooks} del menú Codi i, a continuació, col·loca el personatge a l'espai entre les dues parets.

![captura de pantalla](images/world-door.png)

--- /task ---

--- task ---

Afegeix codi al personatge de la `porta blava` de manera que només sigui visible a l'habitació 3.

--- /task ---

--- task ---

Afegeix codi al personatge de la `porta blava` de manera que, quan la clau es troba a l'`inventari`{:class="block3variables"}, el personatge `s'amaga`{:class="block3looks"} per permetre al teu `jugador` passar.

![porta](images/door.png)

```blocks3
when flag clicked
espera fins <[inventari v] conté [clau blava]?>
atura [altres programes del personatge v]
amaga't
```

--- /task ---

--- task ---

Prova el teu joc i mira si pots recollir la clau blava per obrir la porta!

--- /task ---