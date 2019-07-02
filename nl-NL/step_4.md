## Verplaats je door je wereld

De `speler` sprite zou door deuren naar andere kamers moeten kunnen lopen.

Het project bevat achtergronden voor extra kamers:

![screenshot](images/world-backdrops.png)

\--- task \---

Maak een nieuwe variabele 'voor alle sprites' met de naam `kamer`{:class="block3variables"} om bij te houden in welke kamer de `speler` sprite zich bevindt.

[[[generic-scratch3-add-variable]]]

![screenshot](images/world-room.png) \--- /task \---

\--- task \--- Als de `speler` sprite de oranje deur in de eerste kamer raakt moet de volgende achtergrond worden weergegeven en de `speler` sprite moet teruggaan naar de linkerkant van het speelveld. Voeg deze code toe aan de `speler` sprite's `herhaal`{:class="block3control"} lus:

![speler](images/player.png)

```blocks3
wanneer groene vlag wordt aangeklikt
herhaal 
  als <toets (pijltje omhoog v) ingedrukt? > dan
            richt naar (0) graden
            neem (4) stappen
        einde
        als <toets (pijltje links v) ingedrukt? > dan
            richt naar (-90) graden
            neem (4) stappen
      einde
        als <toets (pijltje omlaag v) ingedrukt? > dan
            richt naar (-180) graden
            neem (4) stappen
        einde
        als <toets (pijltje rechts v) ingedrukt? > dan
            richt naar (90) graden
            neem (4) stappen
        einde
        als < raak ik kleur [#BABABA]? > dan
    neem (-4) stappen
    einde
+ als < raak ik kleur [#F2A24A] > dan
    verander achtergrond naar (volgende achtergrond v)
    ga naar x: (-200) y: (0)
    verander [kamer v] met (1)
    einde
einde
```

\--- /task \---

\--- task \--- Elke keer dat het spel start, moeten de kamer, de positie van het personage en de achtergrond opnieuw ingesteld worden.

Voeg code toe aan de **start** van je `speler` sprite-code boven de `herhaal`{:class="block3control"} lus, om alles opnieuw in te stellen wanneer op de vlag wordt geklikt:

\--- hints \--- \--- hint \--- Wanneer het spel start:

+ De waarde van `kamer`{:class="block3variables"} moet zijn ingesteld op `1`{:class="block3variables"}
+ De `achtergrond`{:class="block3looks"} moet zijn ingesteld op `kamer1`{:class="block3looks"}
+ De positie van de `speler` sprite moet worden ingesteld op `x:-200 y: 0`{:class="block3motion"} \--- / hint \--- \--- hint \--- Dit zijn de extra blokken die je nodig hebt:

![speler](images/player.png)

```blocks3
ga naar x: (-200) y: (0)

maak [kamer v] (1)

verander achtergrond naar (kamer1 v)
```

\--- / hint \--- \--- hint \--- Hier zie je hoe je voltooide script er uit moet zien:

![speler](images/player.png)

```blocks3
wanneer groene vlag wordt aangeklikt
+ maak [kamer v] (1)
+ ga naar x: (-200) y: (0)
+ verander achtergrond naar (kamer1 v)
herhaal
    als <toets (pijltje omhoog v) ingedrukt? > dan
            richt naar (0) graden
            neem (4) stappen
        einde
        als <toets (pijltje links v) ingedrukt? > dan
            richt naar (-90) graden
            neem (4) stappen
      einde
        als <toets (pijltje omlaag v) ingedrukt? > dan
            richt naar (-180) graden
            neem (4) stappen
        einde
        als <toets (pijltje rechts v) ingedrukt? > dan
            richt naar (90) graden
            neem (4) stappen
        einde
        als < raak ik kleur [#BABABA]? > dan
    zet (-4) stappen
    einde
   als < raak ik kleur [#F2A24A] > dan
    verander achtergrond naar (volgende achtergrond v)
    ga naar x: (-200) y: (0)
    verander [kamer v] met (1)
    einde
einde
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \--- Klik op de vlag en verplaats vervolgens je `speler` sprite totdat het de oranje deur raakt. Gaat de sprite naar het volgende scherm? Verandert de variabele `kamer`{:class="block3variables"} naar `2`?

![screenshot](images/world-room-test.png) \--- /task \---