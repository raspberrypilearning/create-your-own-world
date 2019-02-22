## Pevné steny

\--- úloha \--- Vyskúšajte znovu vášho `hráča`. Vidíte, že môže prechádzať cez svetlo sivé steny.

![snímka obrazovky](images/world-walls.png) \--- / úloha \---

\--- \--- úloha Ak chcete tento problém odstrániť, je potrebné, aby sa `hráč` sprite presunúť späť, ak sa dotkne svetlo šedej múru. Tu je kód, ktorý musíte pridať do bloku `navždy`{: class = "block3control"} pod blokmi smerov:

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
+ ak < dotýkať farbu [#BABABA]? > potom
    krok (-4) kroky
    koniec
koniec
```

\--- / úloha \---

\--- úloha \---

Snažte sa, aby sa prehrávač `prehrávača` presunul cez stenu. Ak váš nový kód funguje, nemalo by to byť možné.

![snímka obrazovky](images/world-walls-test.png) \--- / úloha \---