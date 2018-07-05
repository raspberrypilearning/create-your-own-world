## Deuren en sleutels

Hoe zou het zijn als sommige deuren op slot zijn en de speler eerst een sleutel moet hebben om door te kunnen gaan?

+ Neem de sprite `persoon`. Klik er met de rechtermuisknop op en kies **verschijn** zodat het te zien is op het speelveld.

+ Bewerk het uiterlijk van de sprite` sleutel `zodat die blauw is.

+ Ga naar speelveldachtergrond kamer 3 en zet de sprite `sleutel` op een lastig te bereiken plek!
    
    ![screenshot](images/world-key.png)

+ Voeg code toe aan de sprite `sleutel` zodat die alleen in kamer 3 verschijnt.

+ Maak een nieuwe lijst met de naam `inventaris`{: class = "blockdata"}. Hier bewaar je alle dingen die je sprite `speler` verzamelt.

[[[generic-scratch-make-list]]]

+ De code voor het pakken van de sleutel lijkt erg op de code voor het pakken van munten. Het verschil is dat je de sleutel toevoegt aan de inventaris.

```blocks
    wanneer groene vlag wordt aangeklikt
wacht tot <raak ik [speler v] ?>
voeg [blauwe sleutel] toe aan [inventaris v]
stop [andere scripts in sprite v]
verdwijn
```

+ Test de sprite `sleutel` om te zien of je hem kan pakken en toevoegen aan de inventaris. Vergeet niet om code aan het Speelveld toe te voegen om de inventaris leeg te maken aan het begin van het spel.

```blocks
    verwijder item (alle v) van [inventaris v]
```

+ Laten we nu de gesloten deur toevoegen. Klik met de rechtermuisknop op de sprite ` blauwedeur`, selecteer ** verschijn ** en zet de sprite dan in de opening tussen de twee muren.

![screenshot](images/world-door.png)

+ Voeg code toe aan de sprite `blauwedeur` zodat die alleen in kamer 3 te zien is.

+ De sprite `blauwedeur` moet kunnen verdwijnen om de sprite `speler` de doorgang te geven, als die de blauwe sleutel in de inventaris heeft.

```blocks
    wanneer groene vlag wordt aangeklikt
wacht tot <[inventaris v] bevat [blauwe sleutel]?>
stop [andere scripts in sprite v]
verdwijn
```

+ Test je project en kijk of je de blauwe sleutel kunt pakken om de deur te openen!