## Ľudia

Pridajte ďalších ľudí do svojho sveta, s ktorými môže interagovať váš `hráč` sprite.

\--- task \--- Prepnúť na `osobu` sprite.

![Osoba sprite](images/person.png) \--- / úloha \---

\--- úloha \--- Pridajte nejaký kód na `osobu` sprite, aby osoba hovorila s `hráčmi` sprite. Tento kód je veľmi podobný kódu, ktorý ste pridali do vášho `znamenia` sprite:

![človek](images/person.png)

```blocks3
keď vlajka klikne
prejdite na x: (0) y: (-150)
navždy
    ak sa < dotýka (hráč v)? > potom
        povedať [Viete, že môžete prejsť oranžovými a žltými dverami?]
    iný
        povedať []
    koniec
koniec
```

\--- / úloha \---

\--- task \--- Povoľte, aby sa vaša `osoba` sprite pohybovala pridaním týchto dvoch blokov do sekcie `else {`:: class = "block3control"} vášho kódu:

![človek](images/person.png)

```blocks3
keď vlajka klikne
prejdite na x: (0) y: (-150)
navždy
    ak sa < dotýka (hráč v)? > potom
        povedať [Vedeli ste, že môžete prejsť oranžové a žlté dvere?]
    iný
        povedať []
+ pohyb (1) kroky
+ ak na okraji, odskočiť
    koniec
konca

```

\--- / úloha \---

Vaša `osoba` sprite sa teraz bude pohybovať, ale prestane hovoriť s `hráčmi` sprite.

![snímka obrazovky](images/world-person-test.png)

\--- úloha \--- Pridajte kód k svojej novej `osobe` sprite tak, aby sa sprite objavil iba v miestnosti 1. Kód je potrebné je presne rovnaký ako kód, ktorý robí `znamení` sprite iba viditeľnou na izbe 1.

Uistite sa, že vyskúšate nový kód. \--- / úloha \---