## Uși și chei

Acum vei adăuga cod, astfel încât unele dintre ușile din lumea ta să fie încuiate, iar jucătorul trebuie să găsească cheia pentru a le deschide și a ajunge în camera următoare.

\--- task \--- Schimbă la personajul `cheie`. Dă click pe `show`{:class="blocklooks"} în meniul Scripts pentru ca cheia să apară pe scenă. \--- /task \---

\--- task \--- Editează `cheia`, astfel încât să fie albastră. \--- /task \---

\--- task \--- Comutați scena în camera 3 și poziționează `cheia` undeva greu accesibil!

![captură de ecran](images/world-key.png)

\--- /task \---

\--- task \--- Adaugă cod `cheii` tale ca aceasta să fie vizibilă doar în camera 3. \--- /task \---

\--- task \--- Creează o nouă listă denumită `inventory`{:class="block3variables"} pentru a depozita lucrurile pe care `personajul` tău le adună.

[[[generic-scratch3-make-list]]] \--- /task \---

\--- task \--- Codul pe care trebuie să îl adaugi pentru colectarea cheii este similar codului pentru adunarea monezilor. Diferența este că adăugați cheia în `inventory`{:class="block3variables"}.

![cheie](images/key.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
add [blue key] to [inventory v]
hide
stop [other scripts in sprite v]
```

\--- /task \---

\--- task \--- Adaugă cod scenei pentru a goli inventarul la începutul jocului.

```blocks3
delete (all v) of [inventory v]
```

\--- /task \---

\--- task \--- Testează-ți jocul pentru a verifica dacă poți colecta `cheia` și a o adăuga în inventarul tău. \--- /task \---

\--- task \--- Adăugă ușa încuiată. Selectează `ușa albastră` și dă click pe `show`{:class="blocklooks}, apoi așeaz-o peste gaura dintre cei doi pereți.

![captură de ecran](images/world-door.png) \--- /task \---

\--- task \--- Adaugă cod `ușii albastre` ca aceasta să fie vizibilă doar în camera 3. \--- /task \---

\--- task \--- Adaugă cod `ușii albastre` ca atunci când cheia este în `inventory`{:class="block3variables"}, ușa să dispară `hides`{:class="block3looks"} pentru a-i permite `personajului` să treacă.

![uşă](images/door.png)

```blocks3
when flag clicked
wait until <[inventory v] contains [blue key]?>
stop [other scripts in sprite v]
hide
```

\--- /task \---

\--- task \--- Testează-ți jocul pentru a vedea dacă poți colecta cheia albastră pentru a deschide ușa! \--- /task \---