## Zbierať mince

Váš `hráč` by mal byť schopný zbierať mince pri pohybe po celom svete.

\--- task \--- Pridajte novú premennú valled `mince`{: class = "block3variables"} do vášho projektu. \--- / úloha \---

\--- úloha \--- Kliknite pravým tlačidlom na `mincu` a vyberte **zobraziť**.

![snímka obrazovky](images/coin.png) \--- / úloha \---

\--- úloha \--- Pridajte kód do vašej `mince` sprite tak, aby sa objavil iba v miestnosti 1. ![snímka obrazovky](images/coin.png)

```blocks3
keď vlajka klikne
navždy
ak <(miestnosť :: premenné) =[1]> potom
zobraziť
iný
skryť
```

\--- / úloha \---

\--- úloha \---

Pridajte kód do `mince` pohyblivý symbol tak, aby sa vodník `skrýva`{: class = "block3looks"} a `1`{: class = "block3variables"} sa pridá k `mincí`{: class = "block3variables"} premenlivá, akonáhle sa spriete `hráčov` dotýka `mincov` sprite, aby ich "vyzdvihol".

![mince](images/coin.png)

```blocks3
keď vlajka klikne
počká, až <touching (player v)?>
zmení [mince v] podľa (1)
skryť
stop [iné skripty v sprite v]
```

Kód `zastaviť ďalšie skripty v sprite`{: class = "block3control"} je potrebný tak, aby sa `mince` sprite prestane zobrazovať v miestnosti 1 po jeho zhromaždení.

\--- / úloha \---

\--- task \--- Teraz pridajte kód do scény, aby ste nastavili `mincu`{: class = "block3variables"} premennú na `0`{: class = "block3variables"} na začiatku hry.

![štádium](images/stage.png)

```blocks3
keď príznakom kliknete na
nastavíte [mince v] na hodnotu [0]
```

\--- / úloha \---

\--- task \--- Vyskúšajte hru. Zbieranie mince by malo zmeniť `mincí` skóre na `1`{: class = "block3variables"}. \--- / úloha \---