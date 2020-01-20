## Portes i claus

Ara afegiràs codi perquè algunes de les portes del món del joc estiguin bloquejades i el jugador hagi de trobar la clau per obrir-les i arribar a la sala següent.

\--- task \--- Canvia a la tecla icona de `clau `. Fes clic a `mostra` {: class = "blocklooks"} al menú Scripts de manera que la icona aparegui a l'escenari. \--- /task \---

\--- task \--- Edita l'aparença de la icona de `clau` perquè quedi de color blava. \--- /task \---

\--- task \--- Canvia el teló de fons del teu escenari a l'habitació 3 i posa la icona de la `clau` en algun lloc difícil d’arribar!

![captura de pantalla](images/world-key.png)

\--- /task \---

\--- task \--- Afegeix codi a la teva icona de `clau` de manera que només sigui visible a l'habitació 3. \--- /task \---

\--- task \--- Crea una llista nova anomenada ` inventari ` {: class = "block3variables"} per emmagatzemar els articles que el teu `jugador` recull.

[[[generic-scratch3-make-list]]] \--- / tasca \---

\--- task \--- El codi que has d'afegir per recollir la clau és molt similar al codi de recollida de monedes. La diferència és que afegeixes la clau a ` inventari ` {: class = "block3variables"}.

![clau](images/key.png)

```blocks3
quan has fet clic a la bandera
espera fins que <touching (player v)?>
afegeix [clau blava] a [inventari v]
amaga
atura [altres scripts a la icona v]
```

\--- /task \---

\--- task \--- Afegeix codi al teu escenari per buidar l’inventari al començament del joc.

```blocks3
eliminar (tota v) de [inventari v]
```

\--- /task \---

\--- task \--- Prova el teu joc per comprovar si pots recollir la icona ` clau` i afegir-la al teu inventari. \--- /task \---

\--- task \--- Afegeix ara la porta bloquejada. Selecciona la icona ` porta blava ` i fes clic a `mostra ` {: class = "blocklooks} al menú Scripts i, a continuació, col·loca la icona a l'espai entre les dues parets.

![captura de pantalla](images/world-door.png) \--- /task \---

\--- task \--- Afegeix codi a la teva icona de `porta blava` de manera que només sigui visible a l'habitació 3. \--- /task \---

\--- task \--- Afegeix codi a la icona ` porta blava ` de manera que, quan la clau es troba a l' `inventari ` {: class = "block3variables"}, la icona `amaga ` {: class = "block3looks"} per permetre al teu ` jugador` passar.

![porta](images/door.png)

```blocks3
quan has fet clic a la bandera
esperar fins que <[inventari v] contingui [clau blava]?>
aturar [altres scripts a icona v]
amagar
```

\--- /task \---

\--- task \--- Prova el teu joc i mira si pots recollir la clau blava per obrir la porta! \--- /task \---