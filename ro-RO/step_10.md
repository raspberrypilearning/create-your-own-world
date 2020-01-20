## Adună monede

`Personajul` tău ar fi trebui să poată aduna monezi pe măsură ce se deplasează prin lume.

\--- task \--- Adaugă o nouă variabilă, `coins`{:class="block3variables"}, proiectului tău. \--- /task \---

\--- task \--- Alege `moneda` și ăd click pe **show**.

![captură de ecran](images/coin.png) \--- /task \---

\--- task \--- Adaugă cod `monedei` tale ca aceasta să apară doar în camera 1. ![captură de ecran](images/coin.png)

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

Adaugă cod `monedei` tale astfel încât `hides`{:class="block3looks"} și `1`{:class="block3variables"} sunt adăugate variabilei `coins`{:class="block3variables"} atunci când `personajul` atinge `moneda` pentru a o „ridica”.

![monedă](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

Codul `stop other scripts in sprite`{:class="block3control"} este necesar pentru ca `moneda` să nu mai fie afișat în camera 1 după ce a fost colectată.

\--- /task \---

\--- task \--- Acum adaugă cod scenei pentru a seta variabila `coins`{:class="block3variables"} la `0`{:class="block3variables"} la începutul jocului.

![scenă](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

\--- /task \---

\--- task \--- Testează-ți din nou codul. Colectarea unei monede ar trebui să schimbe scorul `monedelor` la `1`{:class="block3variables"}. \--- /task \---