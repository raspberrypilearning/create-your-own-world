## Trdne stene

\--- task \--- Ponovno preizkusi svojo figuro `igralec`. Kot lahko opaziš, se lahko premika svkozi svetlo-sive zidove.

![posnetek zaslona](images/world-walls.png) \--- /task \---

\--- task \--- Da to popraviš, moraš poskrbeti, da segirua `igralec` pomakne nazaj, kadar se dotakne svetlo-sive stene. Takšna je koda, ki jo moraš dodati znotraj bloka `ponavljaj`{:class="block3control"}, pod bloke, ki skrbijo za premikanje:

![igralec](images/player.png)

```blocks3
ko kliknemo na zastavo
ponavljaj
  če <je pritisnjena tipka (puščica gor v)? > potem
    obrni se v smer (0)
    pojdi (4) korakov
  konec
če <je pritisnjena tipka (puščica levo v)? > potem
    obrni se v smer (-90)
    pojdi (4) korakov
  konec
+ če <je pritisnjena tipka (puščica dol v)? > potem
    obrni se v smer (180)
    pojdi (4) korakov
  konec
+ če <je pritisnjena tipka (puščica desno v)? > potem
    obrni se v smer (90)
    pojdi (4) korakov
  konec
+ če < se dotika barve [#BABABA]? > potem
    pojdi (-4) korakov
    konec
konec
```

\--- /task \---

\--- task \---

Poskusi premakniti figuro `igralec` skozi zid. Če tvoja koda deluje, to ne bi smelo biti mogoče.

![posnetek zaslona](images/world-walls-test.png) \--- /task \---