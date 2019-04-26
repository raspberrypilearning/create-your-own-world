## Uitdaging: voeg een vijand toe

Als je wilt, kun je ook patrouillerende vijanden aan je spel toevoegen. Als de `speler` Sprite een vijand raakt, eindigt het spel.

+ Je spel bevat al een `vijand` sprite. Voeg code toe aan de `vijand` sprite zodat deze alleen in kamer 2 verschijnt.

+ Voeg code toe om de `vijand` sprite te laten bewegen en om het spel te stoppen als `vijand` sprite de `speler` sprite raakt. Het is makkelijker om dat in verschillende blokken code te doen. Zo zou de code van de `vijand` sprite eruit kunnen zien:

```blocks3
wanneer groene vlag wordt aangeklikt
herhaal
als <(kamer :: variables)=[2]> dan
vershijn
anders
verdwijn

wanneer groene vlag wordt aangeklikt
herhaal
als <touching (player v)?> dan
stop [alle v]

wanneer groene vlag wordt aangeklikt
ga naar x : (170) y: (0)
herhaal
herhaal (130)
verander x met (-1)
end
herhaal (130)
verander x met (1)
```

+ Test je nieuwe code om ervoor te zorgen dat: 
    + De `vijand` Sprite alleen zichtbaar is in kamer 2
    + De `vijand` sprite door de kamer patrouilleert
    + Het spel eindigt als de `speler` sprite de `vijand` sprite raakt

Kun je nog een`vijand` sprite in kamer 3 maken die op en neer door het gat in de muur beweegt?

![screenshot](images/world-enemy2.png)