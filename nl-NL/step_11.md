## Deuren en sleutels

Now you are going to add code so that some of the doors in your game world are locked, and the player must find the key to open them and get to the next room.

\--- task \--- Schakel over naar de `sleutel` sprite. Klik op `Toon` {:class="blocklooks"} in het Scripts-menu, zodat de sprite in het werkgebied verschijnt. \--- /task \---

\--- task \--- Bewerk het uiterlijk van de `sleutel` sprite zodat die blauw is. \--- /task \---

\--- taak \--- Verander je achtergrond naar kamer 3 en plaats de `sleutel` sprite ergens waar hij moeilijk te bereiken is!

![screenshot](images/world-key.png)

\--- /task \---

\--- task \--- Voeg code toe aan je nieuwe `sleutel` sprite zodat de sprite alleen in kamer 3 verschijnt. \--- /task \---

\--- task \--- Maak een nieuwe lijst met de naam `inventaris` {:class="block3variables"} om de items die je `speler` sprite verzamelt op te slaan.

[[[generic-scratch3-make-list]]] \--- /task \---

\--- task \--- De code die je moet toevoegen voor het verzamelen van de sleutel lijkt sterk op de code voor het verzamelen van munten. Het verschil is dat je de sleutel toevoegt aan de `inventaris` {:Class="block3variables"}.

![sleutel](images/key.png)

```blocks3
wanneer groene vlag wordt aangeklikt
wacht tot <touching (player v)?>:: control
voeg [sleutel] toe aan [inventaris v]:: list
verdwijn:: looks
stop [andere scripts in sprite v]:: control
```

-- /task \---

\--- taak \--- Voeg code aan je werkgebied toe om je inventaris aan het begin van het spel te legen.

```blocks3
verwijder item (alle v) van [inventaris v]:: list
```

\--- /task \---

\--- task \--- Test je spel om te controleren of je de `sleutel` kunt verzamelen en aan je inventaris wordt toegevoegd. \--- /task \---

\--- task \--- Voeg nu de vergrendelde deur toe. Selecteer de `blauwedeur` sprite en klik op `toon`{:class="blocklooks} in het sprite menu, en plaats vervolgens de sprite in het gat in de vertikale muur.

![screenshot](images/world-door.png) \--- /task \---

Voeg code toe aan de `blauwedeur` sprite zodat die alleen in kamer 3 te zien is. \--- /task \---

\--- taak \--- Voeg code aan de `blauwedeur` sprite toe zodat wanneer de sleutel in de `inventaris`{:class="block3variables"} staat, de deur zich `verbergt`{:class="block3looks"} zodat je `speler` de doorgang kan passeren.

![deur-](images/door.png)

```blocks3
wanneer groene vlag wordt aangeklikt
wacht tot <[inventaris v] bevat [blauwesleutel]?:: list>:: control
stop [andere scripts in sprite v]:: control
verdwijn:: looks
```

\--- /task \---

\--- task \--- Test je spel en kijk of je met het verzamelen van de blauwe sleutel de deur kunt openen! \--- /task \---