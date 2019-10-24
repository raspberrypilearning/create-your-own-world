## Značky

Teraz pridajte značky do vášho sveta, aby ste sa naučili hráčov na ich ceste.

Váš projekt obsahuje `vítaný znak` sprite:

![snímka obrazovky](images/world-sign.png)

\--- úloha \--- `vítaný znak` sprite by mal byť viditeľný len v miestnosti 1, takže pridajte nejaký kód do sprite, aby ste sa uistili, že k tomu dôjde:

\--- pokyny \--- \--- tip \--- `Keď sa na vlajku klikne`{: class = "block3events"}, v smere `navždy`{: class = "block3control"}, začiarknite `ak`{: class = "block3control"} na `izbe je 1`{: class = "block3variables"} a v tomto prípade `ukazujú,`{: class = "block3looks"} `uvítací tabule` vodník, `ešte`{: class = "block3control"} `skryť`{: class = "block3looks"} Sprite. \--- / hint \--- \--- hint \--- Tu sú bloky, ktoré potrebujete:

![znamenie](images/sign.png)

```blocks3
<br />ak < > potom
iný
koniec

< (miestnosť :: premenné) = [1] >

skryť

zobraziť

navždy
koniec

keď klepol vlajku

```

\--- / hint \--- \--- hint \--- Tu je kompletný kód:

![znamenie](images/sign.png)

```blocks3
keď vlajka klikne
navždy
    ak < (miestnosť :: premenné) = [1] > potom
        zobraziť
    iný
        skryť
    koniec
koniec
```

\--- / tip \--- \--- / tipy \---

\--- / úloha \---

\--- task \--- Vyskúšajte kód pre svoj `vítaný znak` sprite pohybom medzi miestnosťami. Značka by mala byť viditeľná iba v miestnosti 1.

![snímka obrazovky](images/world-sign-test.png) \--- / úloha \---

\--- task \--- Znak nie je moc dobrý, ak nehovorí nič! Pridajte trochu viac kódu pre zobrazenie správy v prípade, že `vítanou známkou` sprite sa dotýka `hráča` sprite:

![znamenie](images/sign.png)

```blocks3
keď sa klavírka na
navždy
ak < (miestnosť :: premenné) = [1] > potom
zobrazuje
iný
skryť
koniec
+ ak sa < dotýka (hráč v)? > potom
povedzte [Vitajte! Môžete sa dostať k pokladu?]
iný
povedať []
koniec
koniec
```

\--- / úloha \---

\--- úloha \--- Vyskúšajte svoje `vítané znamenie` Sprite znovu. Teraz by ste mali vidieť správu, keď sa prehrávač `prehrávača` dotýka `vítaných znamienok` sprite.

![snímka obrazovky](images/world-sign-test2.png) \--- / úloha \---