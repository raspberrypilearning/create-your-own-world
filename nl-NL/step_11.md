## Deuren en sleutels

Nu ga je code toevoegen zodat sommige van de deuren in je spelwereld op slot zijn en de speler de sleutel moet vinden om ze te openen en naar de volgende kamer te gaan.

--- task --- Schakel over naar de `sleutel` sprite. Klik op `verschijn`{:class="block3looks"} in het Scripts-menu, zodat de sprite in het werkgebied verschijnt. --- /task ---

--- task --- Bewerk het uiterlijk van de `sleutel` sprite zodat die blauw is. --- /task ---

--- task --- Verander je achtergrond naar kamer 3 en plaats de `sleutel` sprite ergens waar hij moeilijk te bereiken is!

![screenshot](images/world-key.png)

--- /task ---

--- task --- Voeg code toe aan je nieuwe `sleutel` sprite zodat de sprite alleen in kamer 3 verschijnt. --- /task ---

--- task --- Maak een nieuwe lijst met de naam `inventaris`{:class="block3variables"} om de items die je `speler` sprite verzamelt op te slaan.

[[[generic-scratch3-make-list]]] --- /task ---

--- task --- De code die je moet toevoegen voor het verzamelen van de sleutel lijkt sterk op de code voor het verzamelen van munten. Het verschil is dat je de sleutel toevoegt aan de `inventaris`{:class="block3variables"}.

![sleutel](images/key.png)

```blocks3
wanneer groene vlag wordt aangeklikt
wacht tot <touching (player v)?>
voeg [blauwe sleutel] toe aan [inventaris v]
verdwijn
stop [andere scripts in sprite v]
```

--- /task ---

--- task --- Voeg code aan je werkgebied toe om je inventaris aan het begin van het spel te legen.

```blocks3
verwijder item (alle v) van [inventaris v]:: list
```

--- /task ---

--- task --- Test je spel om te controleren of je de `sleutel` kunt verzamelen en aan je inventaris toegevoegen. --- /task ---

--- task --- Voeg nu de vergrendelde deur toe. Selecteer de `blauwe deur` sprite en klik op `verschijn`{:class="block3looks} in het sprite menu, en plaats vervolgens de sprite in het gat in de vertikale muur.

![screenshot](images/world-door.png) --- /task ---

--- task --- Voeg code toe aan de `blauw deur` sprite zodat die alleen in kamer 3 te zien is. --- /task ---

--- task --- Voeg code aan de `blauwe deur` sprite toe zodat wanneer de sleutel in de `inventaris`{:class="block3variables"} staat, de deur zich `verbergt`{:class="block3looks"} zodat je `speler` de doorgang kan passeren.

![deur](images/door.png)

```blocks3
wanneer groene vlag wordt aangeklikt
wacht tot <[inventaris v] bevat [blauwe sleutel]?>
stop [andere scripts in sprite v]
verdwijn
```

--- /task ---

--- task --- Test je spel en kijk of je met het verzamelen van de blauwe sleutel de deur kunt openen! --- /task ---