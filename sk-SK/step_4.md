## Presuňte sa okolo sveta

Hráč `hráč` by mal byť schopný prejsť dverami do iných miestností.

Váš projekt obsahuje pozadie ďalších izieb:

![snímka obrazovky](images/world-backdrops.png)

\--- úloha \---

Vytvorenie nového, pre všetky škriatkov 'premenné nazvané `izba`{: class = "block3variables"}, aby mohli sledovať, ktorá izbe `hráč` sprite nachádza.

[[[generic-scratch3-add-variable]]]

![snímka obrazovky](images/world-room.png) \--- / úloha \---

\--- \--- úloha Keď `hráč` sprite dotkne oranžovej dvere v prvej miestnosti, hra by mala zobraziť ďalšie pozadia a `hráč` sprite by sa mal pohybovať späť na ľavej strane plochy. Pridajte tento kód vo vnútri prehrávača `prehrávača` navždy `sprite <code>`= {block3control}}:

![prehrávač](images/player.png)

```blocks3
keď sa vlajka preklikne
navždy
    ak <stlačíte tlačidlo (šípka nahor v)? > potom
        bod v smere (0)
        posunúť (4) kroky
    koniec
    ak je stlačené tlačidlo <(šípka doľava v)? > potom
        bod v smere (-90)
        posunúť (4) kroky
    koniec
        ak stlačíte klávesu <(šípka dole v)? > potom
        bod v smere (-180)
        posunúť (4) kroky
    koniec
        ak je stlačené tlačidlo <[šípka vpravo v]? > potom
        bod v smere (90)
        posunúť (4) kroky
    koniec
    ak < dotýkať farbu [#BABABA]? > potom
    ťah (-4), kroky
    koniec
+ v prípade < dotýkať farieb [# F2A24A] > potom
    prepínač pozadia k (ďalší v pozadí)
    prejdite na X: (-200) y: (0)
    zmena [izbu v] od (1)
    koniec
konca
```

\--- / úloha \---

\--- úloha \--- každom spustení hry je potrebné resetovať miestnosť, pozíciu znakov a pozadie.

Pridajte kód **štartu** vašej `hráči` sprite kódu nad `navždy`{: class = "block3control"} slučky, resetovať všetko, keď je príznak spúšťanie:

\--- tipy \--- \--- tip \--- Keď začne hra:

+ Hodnota `miestnosti`{: class = "block3variables"} by mala byť nastavená na `1`{: class = "block3variables"}
+ `pozadie`{: class = "block3looks"} by malo byť nastavené na `miestnosti1`{: class = "block3looks"}
+ Poloha `hráča` by mala byť nastavená na `x: -200 y: 0`{: class = "block3motion") \--- / hint \--- \--- tip \--- Tu sú extra bloky, ktoré potrebujete:

![prehrávač](images/player.png)

```blocks3
prejdite na x: (-200) y: (0)

nastavte [miestnosť v] na (1)

spínaciu plochu do (miestnosť v)
```

\--- / hint \--- \--- hint \--- Tu je to, ako by mal vyzerať váš hotový skript:

![prehrávač](images/player.png)

```blocks3
keď príznak kliknutí
+ sada [miestnosti] pre (1)
+ prejsť na x: (-200) y: (0)
+ prepnúť kulisu (pokoj1 v)
navždy
    , pokiaľ <tlačidlo (šípka hore V) stlačené ? > potom
        bod v smere (0)
        posunúť (4) kroky
    koniec
    ak je stlačené tlačidlo <(šípka doľava v)? > potom
        bod v smere (-90)
        posunúť (4) kroky
    koniec
        ak stlačíte klávesu <(šípka dole v)? > potom
        bod v smere (-180)
        posunúť (4) kroky
    koniec
        ak je stlačené tlačidlo <[šípka vpravo v]? > potom
        bod v smere (90)
        posunúť (4) kroky
    koniec
    ak < dotýkať farbu [#BABABA]? > potom
    ťah (-4), kroky
    koniec
    v prípade, < dotýkať farba [# F2A24A] > potom
    prepínač pozadia k (ďalší v pozadí)
    prejdite na X: (-200) y: (0),
    zmena [miestnosti V ] do (1)
konca
konca
```

\--- / tip \--- \--- / tipy \---

\--- / úloha \---

\--- task \--- Kliknite na vlajku a potom presuňte vášho `hráča` až kým sa nedotkne oranžových dverí. Sprievod sa presunie na ďalšiu obrazovku? Zmenila sa premenná `miestnosti`{: class = "block3variables"} na `2`?

![snímka obrazovky](images/world-room-test.png) \--- / úloha \---