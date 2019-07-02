## Personen

Laten we andere personen aan je wereld toevoegen waarmee de `speler` sprite kan communiceren.

\--- task \--- Schakel over naar de `persoon` sprite.

![Person sprite](images/person.png) \--- /task \---

\--- task \--- Voeg wat code toe aan de `persoon` sprite zodat deze spreekt met de `speler` sprite. Deze code zal erg lijken op de code die je aan je `welkomstbord` sprite hebt gegeven:

![persoon](images/person.png)

```blocks3
wanneer groene vlag wordt aangeklikt
ga naar x: (0) y: (-150)
herhaal 
  als < raak ik (speler v)? > dan 
    zeg [Wist je dat je door de oranje en gele deuren kunt gaan?]
  anders
    zeg []
  einde
einde
```

\--- /task \---

\--- task \--- Sta je `persoon` sprite toe zich te verplaatsen door deze twee blokken in het `anders`{:class="block3control"} gedeelte van je code toe te voegen:

![persoon](images/person.png)

```blocks3
wanneer groene vlag wordt aangeklikt
ga naar x: (0) y: (-150)
herhaal 
  als <raak ik (speler v)?> dan  &gt; dan 
    zeg [Wist je dat je door de oranje en gele deuren kunt gaan?]
  anders
    zeg []
+   neem (1) stappen
+   keer om aan de rand
  einde
einde

```

\--- /task \---

De sprite `persoon` zal nu gaan bewegen maar stopt om te spreken met `speler` sprite.

![screenshot](images/world-person-test.png)

\--- task \--- Voeg code toe aan je nieuwe `persoon` sprite zodat de sprite alleen in kamer 1 verschijnt. De code die je nodig hebt, is exact dezelfde als de code waardoor de `welkomstbord` sprite alleen zichtbaar is in kamer 1.

Zorg ervoor dat je je nieuwe code test. \--- /task \---