## Skupljaj novčiće

Vaš ` igrač ` sprite bi trebao biti u mogućnosti skupljati novčiće dok se kreće svijetom.

\--- task \---

Dodajte novu varijablu, promjenjivog broja ` kovanice` {: class = "block3variables"} u svoj projekt.

\--- /task \---

\--- task \---

Odaberite ` novčić ` sprite i kliknite ** prikaži **,.

![snimka zaslona](images/coin.png)

\--- /task \---

\--- task \---

Dodajte kôd ` novčić ` sprite tako da se pojavljuje samo u sobi 1.

![snimka zaslona](images/coin.png)

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

Dodajte kôd ` novčić` spriteu tako da se ` skriva ` {: class = "block3looks"} i ` 1 ` {: class = "block3variables"} se pribraja u varijablu ` kovanice` {: class = "block3variables"} kada sprite ` igrač ` dodiruje ` novčić ` i "pokupi ga".

![novčić](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

Kod ` zaustavlja ostale skripte u spriteu ` {: class = "block3control"} potreban je tako da ` novčić ` sprite prestaje biti prikazan u sobi 1 nakon što je prikupljen.

\--- /task \---

\--- task \---

Sada dodajte kôd u Pozornicu da biste postavili varijablu ` kovanice ` {: class = "block3variables"} na ` 0 ` {: class = "block3variables"} na početku igre.

![pozornica](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

\--- /task \---

\--- task \---

Testirajte svoju igru. Prikupljanje novčića trebalo bi promijeniti vaše ` kovanice ` rezultat na ` 1 ` {: Class = "block3variables"}.

\--- /task \---