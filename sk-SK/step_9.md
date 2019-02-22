## Výzva: pridajte nepriateľa

Ak chcete, môžete do svojej hry pridať hliadkovanie nepriateľov. Ak sa hráč `hráča` dotkne nepriateľa, hra končí.

+ Vaša hra už obsahuje `nepriateľa` sprite. Pridajte kód na `nepriateľa` sprite tak, aby sa objavil iba v miestnosti 2.

+ Pridajte kód pre presunutie `nepriateľa` sprite a pre ukončenie hry, ak sa `nepriateľské` sprite dotýka `hráčov` sprite. Je to jednoduchšie v samostatných kódových blokoch. Tu je návod, ako môže vyzerať váš `nepriateľský kód`:

```blocks3
keď vlajka klikne
navždy
ak <(miestnosť :: premenné) =[2]> potom
ukáže
iný
skryť

keď vlajka klikne
navždy
ak <touching (player v)?> potom
zastaví [všetko v]

keď príznakom klikni
prejdite na x: ( 170) y: (0)
navždy
opakovanie (130)
zmena x od (-1)
koniec
opakovanie (130)
zmena x podľa (1)
```

+ Vyskúšajte nový kód, aby ste sa uistili, že: 
    + `nepriateľ` sprite viditeľné len v izbe 2
    + `nepriateľ` sprite hliadky v miestnosti
    + Hra končí, ak je `hráč` sprite dotkne `nepriateľ` sprite

Môžete vytvoriť ďalšie `nepriateľa` sprite v miestnosti 3, ktorá hliadku hore a dole cez medzeru v stene?

![snímka obrazovky](images/world-enemy2.png)