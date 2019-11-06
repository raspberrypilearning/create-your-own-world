## Zbiraj kovance

Tvoja figura `igralec` bi moral imeti možnost, da zbira kovance, ko se sprehaja po svetu.

\--- task \--- Dodaj novo spremenljivko z imenom `kovanci`{:class="block3variables"} v tvoj projekt. \--- /task \---

\--- task \--- Izberi figuro `kovanec` in klikni na oko zraven napisa **Pokaži**.

![posnetek zaslona](images/coin.png) \--- /task \---

\--- task \--- Figuri `kovanec` dodaj kodo, zaradi katere se bo pojavil zgolj v prvi sobi. ![posnetek zaslona](images/coin.png)

```blocks3
ko kliknemo na zastavo
ponavljaj
če <(soba :: Spremenljivka)=[1]> potem
pokaži
sicer
skrij
```

\--- /task \---

\--- task \---

Figuri `kovanec` dodaj kodo, da se bo figura `skrila`{:class="block3looks"} in dodala `1`{:class="block3variables"} spremenljivki `kovanci`{:class="block3variables"}, ko se figura `igralec` dotakne figure `kovanec`, da jo 'pobere'.

![kovanec](images/coin.png)

```blocks3
ko kliknemo na zastavo
počakaj dokler ni < se dotika (igralec v)?>
spremeni [kovanci v] za (1)
skrij
ustavi [ostale ukaze za to figuro v]
```

Koda `ustavi ostale ukaze za to figuro`{:class="block3control"} je potrebna, da se figura `kovanec` preneha prikazovati v sobi 1, potem ko je pobrana.

\--- /task \---

\--- task \--- Zdaj dodaj kodo v oder, da nastavi spremenljivko `kovanci`{:class="block3variables"} na `0`{:class="block3variables"}, ko se igra začne.

![oder](images/stage.png)

```blocks3
ko kliknemo na zastavo
nastavi [kovanci v] na (0)
```

\--- /task \---

\--- task \--- Preizkusi svojo igro. Ko pobereš kovanec, bi se moralo število `kovanci` povečati na `1`{:class="block3variables"}. \--- /task \---