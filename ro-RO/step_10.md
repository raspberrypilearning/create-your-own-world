## Adună monede

Personajul tău `jucător` ar trebui să poată aduna monezi pe măsură ce se deplasează prin lume.

\--- task \---

Adaugă o nouă variabilă numită `monede`{:class="block3variables"} la proiectul tău.

\--- /task \---

\--- task \---

Selectează personajul `monedă` și dă click pe **arată**.

![captură de ecran](images/coin.png)

\--- /task \---

\--- task \---

Adaugă cod personajului tău `monedă`, astfel încât acesta să apară doar în camera 1.

![captură de ecran](images/coin.png)

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

Adaugă cod personajului tău `monedă`, astfel încât personajul se `ascunde`{:class="block3looks"} și `1`{:class="block3variables"} să fie adăugat la variabila `monede`{:class="block3variables"} odată ce personajul `jucător` atinge personajul `monedă` pentru a-l colecta.

![monedă](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

Codul `stop alte scripturi pentru personaj`{:class="block3control"} este necesar pentru ca personajul `monedă` să nu mai fie afișat în camera 1 după ce a fost colectat.

\--- /task \---

\--- task \---

Acum adaugă codul la Scenă pentru a seta variabila `monede`{:class="block3variables"} la `0`{:class="block3variables"} la începutul jocului.

![scenă](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

\--- /task \---

\--- task \---

Testează-ți jocul. Colectarea unei monede ar trebui să schimbe scorul variabilei `monede` la `1`{:class="block3variables"}.

\--- /task \---